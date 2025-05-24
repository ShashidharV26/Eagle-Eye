# 🦅 Eagle Eye

## 📱 Overview

**Eagle Eye** is a B2B Android mobile application designed specifically for **Touring Talkies operators** and their **bus drivers**. The platform enables drivers to record and upload daily video reports of bus conditions, allowing operators to monitor their fleet remotely without needing to physically visit each bus. Videos are tagged with location and timestamp metadata, offering operators real-time insights into service quality and maintenance standards.

---

## 👥 User Roles

### 🔑 Operator Login
- View and manage all assigned buses.
- Review daily and historical video uploads from each bus.
- Assign buses to drivers.
- Share, comment, and chat with drivers regarding video uploads.
- Monitor compliance and service standards remotely.
- Managed via Touring Talkies subscription plans.

### 🔐 Driver Login
- View only their assigned buses.
- Upload videos under predefined categories: **Interior** and **Exterior**.
- Limited to a specific number of uploads per day per bus based on subscription.
- Automatic video location tagging during recording.
- Add comments and submit videos to the cloud.
- Receive operator feedback via in-app chat.

---

## 🎯 Key Features

- 🔁 **Dual Login Support**: Operators and Drivers with role-based access.
- 🎥 **Video Capture with Metadata**: Capture interior/exterior videos with automatic GPS tagging and timestamps.
- ☁️ **Cloud Uploads**: AWS integration for secure and scalable video storage.
- 📋 **Video Categories & Limits**: Custom video types and quota-based uploads.
- 📍 **Real-Time Location Capture**: Background GPS tracking during recording.
- 🔊 **Push Notifications**: Real-time alerts for video uploads using OneSignal.
- 💬 **In-App Chat**: Per-video chat between operator and driver.
- ⚠️ **Subscription Enforcement**: Access restrictions based on subscription status.
- 🔧 **Admin Control**: Touring Talkies can revoke access based on subscription.

---

## 🛠 Tech Stack

| Feature Area             | Technology Used               |
|--------------------------|-------------------------------|
| Language                 | Kotlin                        |
| UI Framework             | Jetpack Compose + Material 3  |
| Architecture             | MVVM                          |
| Networking               | Retrofit2                     |
| Background Work          | WorkManager                   |
| Video Compression        | FFmpegKit                     |
| Dependency Injection     | Hilt                          |
| Local Storage            | DataStore Preferences         |
| Media Playback           | Media3 Library                |
| Location Services        | Kotlin Coroutines + Fused API |
| Cloud Upload             | AWS Android SDK               |
| Notifications            | OneSignal                     |
| Crash Reporting          | Firebase Crashlytics          |

---

## 🔒 Subscription Handling

- Operators are granted features based on the plan chosen via **Touring Talkies Support**.
- Limits include:
  - Max videos/day
  - Max recording time/video
  - Storage limits
- If subscription expires or is disabled:
  - Operator is blocked.
  - All drivers under that operator lose access.
  - Access resumes upon plan renewal.

---

---

## 📬 Notifications

- Video uploads notify operators via **OneSignal Push Notifications**.
- In-app chat is available for contextual discussions per video.

---

## 🚀 My Contributions

- ✅ Designed and developed the **entire app** from scratch.
- ✅ Built the complete **backend database schema**.
- ✅ Integrated **AWS**, **FFmpegKit**, **WorkManager**, and more.
- ✅ Led the architecture design using **MVVM + Hilt**.
- ✅ Implemented **crash monitoring**, **video compression**, and **cloud sync**.

---

## 🧠 Future Improvements

- Add biometric login for enhanced driver security.
- Dashboard with analytics on bus condition trends.
- Multi-language support for regional drivers/operators.
- Offline video upload queue with sync on connectivity.

---
