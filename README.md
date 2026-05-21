# 🎓 College Event Management System

![Platform](https://img.shields.io/badge/Platform-Android-brightgreen)
![Language](https://img.shields.io/badge/Language-Java-orange)
![Backend](https://img.shields.io/badge/Backend-Firebase-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Min SDK](https://img.shields.io/badge/Min%20SDK-API%2024-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

> A fully functional Android application for managing college events 
> and student registrations — built with Java, XML, Firebase Realtime 
> Database, and Firebase Authentication.

---

## 📱 App Overview

College Event Management System allows students to browse upcoming 
college events, register with smart forms, receive QR code tickets, 
and share confirmations on WhatsApp. Faculty admins can manage all 
registrations in real time, search, filter, and export data. A built-in 
calendar highlights event dates and a venue booking system prevents 
double-booking conflicts.

---

## ✨ Features

### 👨‍🎓 Student Features
- 🔐 Secure login and registration via Firebase Authentication
- 📅 Browse 5 upcoming college events on a clean dashboard
- 🔍 Search events by name using live search bar
- 👥 See registration count per event in real time
- 📋 View full event details — name, date, venue, description
- ⚠️ Venue conflict warning if hall is already booked
- 📝 Smart registration form with:
  - Branch dropdown (IT, AI ML, CE, CS)
  - Year dropdown (1st to 4th Year)
  - 10-digit phone number validation
  - Duplicate registration prevention
- ✅ Confirmation page with unique Registration ID
- 📲 QR Code ticket generated after registration
- 💬 Share confirmation and QR ticket on WhatsApp

### 👨‍💼 Admin Features
- 🔐 Separate admin login (secured credentials)
- 📊 View all registrations in real time
- 🔍 Search by name, phone, or branch
- 🗂️ Filter registrations by event type
- 📤 Export and share data in Excel/text format
- 🗑️ Delete individual registrations
- 📈 Total registration count across all events

### 📅 Calendar Feature
- Monthly calendar view with navigation
- Red highlights on event dates
- List of events for current month displayed below calendar
- Today's date highlighted separately

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Java | Primary programming language |
| XML | UI layout design |
| Android Studio | IDE |
| Firebase Authentication | Student login and registration |
| Firebase Realtime Database | Store and fetch registrations |
| ZXing Library | QR code generation |
| CardView | Premium event card UI |
| AlertDialog | Branch and year dropdowns |
| ListView | Registration list in admin panel |
| Intent | Navigation between all screens |

---

---

## ⚙️ Setup and Installation

### Prerequisites
- Android Studio (Hedgehog or later)
- Firebase account
- Android device or emulator (API 24+)
- Internet connection for first Gradle sync

### Step 1 — Clone the repository
```bash
git clone https://github.com/yourusername/CollegeEventManagement.git
cd CollegeEventManagement
```

### Step 2 — Firebase Setup
1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create new project → name it `CollegeEvents`
3. Add Android App → package: `com.example.myapplicationproject`
4. Download `google-services.json`
5. Place it inside the `app/` folder

### Step 3 — Enable Firebase Services
- **Authentication** → Sign-in method → Enable Email/Password
- **Realtime Database** → Create database → Start in test mode

### Step 4 — Add Firebase Rules (for testing)
```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

### Step 5 — Open in Android Studio

### Step 6 — Run the app

## 🔐 Admin Login Credentials
Email    : admin@college.com
Password : admin123


## 🔮 Future Improvements

- [ ] 🔔 Push notifications via Firebase Cloud Messaging
- [ ] 🔑 Forgot password via email reset
- [ ] 👨‍💼 Admin can dynamically add and delete events
- [ ] 💳 Payment gateway for paid events (Razorpay)
- [ ] 📍 Google Maps integration for venue navigation
- [ ] 📤 Export registrations as PDF or Excel file
- [ ] 📱 OTP based login via Firebase Phone Auth
- [ ] 🌙 Dark mode support
- [ ] 📊 Registration statistics with bar charts

---

## 👥 Team Members

Pranav Patil 
Mohit Patil

---

## 📚 Subject Details

> **Subject:** Mobile Application Development (MAD)
> **Academic Year:** 2025-26
> **Semester:** VI
> **Branch:** Information Technology
> **College:** [NMIMS]
