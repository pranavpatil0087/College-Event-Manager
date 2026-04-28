# 🎓 College Event Management System

![Android](https://img.shields.io/badge/Platform-Android-green)
![Java](https://img.shields.io/badge/Language-Java-orange)
![Firebase](https://img.shields.io/badge/Backend-Firebase-yellow)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![SDK](https://img.shields.io/badge/Min%20SDK-24-blue)

> A fully functional Android application for managing college events 
> and student registrations — built using Java, XML and Firebase.

---

## 📱 Screenshots

> Login → Dashboard → Event Details → Registration → Confirmation → Admin Panel

---

## 🚀 Features

### 👨‍🎓 Student Side
- 🔐 Register and Login using Firebase Authentication
- 📅 View 5 upcoming college events on Dashboard
- 📋 View complete Event Details (name, date, venue, description)
- 📝 Register for any event with smart form
  - Branch dropdown (IT, AI ML, CE, CS)
  - Year dropdown (1st to 4th Year)
  - Phone number validation
- ✅ Confirmation page with unique Registration ID (EVTxxxxx)
- 🔄 Duplicate registration prevention

### 👨‍💼 Admin Side
- 🔐 Secure Admin Login (separate from student login)
- 📊 View all registrations in real time
- 🔍 Search registrations by name, phone or branch
- 🗂️ Filter registrations event-wise
- 📤 Share complete registration list via any app
- 🗑️ Delete individual registrations
- 📈 Total registration count display

---

## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| **Java** | Primary programming language |
| **XML** | UI Layout design |
| **Android Studio** | IDE |
| **Firebase Authentication** | Student login & registration |
| **Firebase Realtime Database** | Store & retrieve registrations |
| **CardView** | Event cards on Dashboard |
| **AlertDialog** | Branch & Year dropdowns |
| **ListView** | Display registrations in Admin |
| **Intent** | Navigation between screens |

---

## 📁 Project Structure
app/
├── java/com/example/myapplicationproject/
│   ├── LoginActivity.java
│   ├── RegisterActivity.java
│   ├── DashboardActivity.java
│   ├── EventDetailActivity.java
│   ├── RegistrationFormActivity.java
│   ├── ConfirmationActivity.java
│   ├── AdminPanelActivity.java
│   └── Event.java
│
└── res/
├── layout/
│   ├── activity_main.xml
│   ├── activity_register.xml
│   ├── activity_dashboard.xml
│   ├── activity_event_detail.xml
│   ├── activity_registration_form.xml
│   ├── activity_confirmation.xml
│   ├── activity_admin_panel.xml
│   └── item_registration.xml
└── values/
├── strings.xml
├── colors.xml
└── themes.xml

## 🔥 Firebase Structure
registrations/
├── Seminar/
│   └── -uniqueKey/
│       ├── name: "Rahul Patil"
│       ├── branch: "CE - Computer Engineering"
│       ├── year: "3rd Year"
│       ├── phone: "9876543210"
│       ├── eventName: "Career Guidance Seminar"
│       ├── registrationId: "EVT28492"
│       └── timestamp: "1716789000000"
├── Workshop/
├── Tech Fest/
├── Hackathon/


## 📲 App Flow
Launch
└── LoginActivity
├── New User → RegisterActivity → DashboardActivity
├── Student Login → DashboardActivity
│     └── Select Event → EventDetailActivity
│           └── Register → RegistrationFormActivity
│                 └── Submit → ConfirmationActivity
│                       └── Back → DashboardActivity
└── Admin Login → AdminPanelActivity
└── Cultural/
