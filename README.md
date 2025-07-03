# CareConnect

---

## Table of Contents
- [Project Description](#project-description)
- [Technical Stack & Architecture](#-technical-stack--architecture)
- [Key Features](#key-features)
  - [Older Adults](#older-adults)
  - [Caregivers](#caregivers)
  - [Family Members](#family-members)
  - [Administrators](#administrators)
- [Setup](#-setup)

---

## Project Description

**CareConnect** is an Android application built to support elderly care through real-time monitoring, communication, and task management. The app empowers older adults to log their daily health activities, follow medication schedules, and request immediate help during emergencies. At the same time, it provides family members and professional caregivers with tools to remotely monitor and manage care, ensuring peace of mind and proactive support.

The system is designed with a multi-role structure — older adults, caregivers, family members, and administrators — each with customized features and access levels. Through Firebase integration, the app ensures secure authentication, real-time data synchronization, and cloud storage capabilities.

CareConnect aims to improve the quality of life for seniors by promoting safety, accountability, and connected care in a user-friendly and scalable solution.

---

## Technical Stack & Architecture

- **Language**: Kotlin
- **UI Toolkit**: Jetpack Compose
- **Backend & Database**: Firebase
  - **Firebase Authentication** – secure multi-role user management
  - **Cloud Firestore** – real-time NoSQL database
  - **Firebase Storage** – profile image storage
- **Navigation**: Jetpack Navigation Compose

---

## Key Features

### Older Adults
- Perform morning and evening check-ins to confirm well-being.
- View and manage daily assigned tasks.
- Track medications and confirm intake.
- Log water consumption and meals for hydration and nutrition tracking.
- Use an SOS button to instantly alert caregivers and family members in emergencies.
- See a list of all connected caregivers and family members.

### Caregivers
- Monitor real-time status of linked patients through a central dashboard.
- Link and manage patients by email.
- Access detailed patient profiles with health data and alerts.
- Add and modify tasks and medications remotely.
- Receive push notifications for missed check-ins, tasks, medications, or SOS events.

### Family Members
- View a dashboard summarizing relatives’ health and activity.
- Get notified about emergencies or missed tasks.
- Access reports with detailed patient information.
- Manage and oversee caregiver relationships.

### Administrators
- Visualize platform activity with user stats by role.
- Search, remove, or promote user accounts.
- Monitor overall user distribution and system usage.

---

## Setup

Follow the instructions below to set up and run the project locally.

### Prerequisites

- [Android Studio](https://developer.android.com/studio) (latest stable version)
- Android SDK 33 or higher
- A Firebase account: [https://firebase.google.com](https://firebase.google.com)
- Git installed

---

### Firebase Configuration

1. **Clone the Repository**
   ```bash
   git clone https://github.com/miguelcorreia01/careconnect-mobile.git
   cd careconnect-mobile
   ```

2. **Create a Firebase Project**
   - Go to [Firebase Console](https://console.firebase.google.com/)
   - Click **"Add project"** and follow the setup steps

3. **Register the Android App**
   - Inside Firebase, click **"Add app" → Android**
   - Enter your Android package name (as found in `AndroidManifest.xml`)
   - Download the `google-services.json` file

4. **Add `google-services.json` to Your Project**
   - Move the file into the `app/` directory of your project:
     ```
     careconnect-mobile/app/google-services.json
     ```

5. **Enable Firebase Services**
   - In the Firebase console:
     - Enable **Authentication** (Email/Password)
     - Enable **Cloud Firestore**
     - Enable **Firebase Storage**

---

### Run the App

1. Open the project in **Android Studio**
2. Let **Gradle** sync and install dependencies
3. Connect an emulator or physical Android device
4. Click **Run**

---
