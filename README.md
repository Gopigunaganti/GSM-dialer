# 📱 GSM Predictive Dialer App – README

## 🚀 Overview
This is a GSM-based auto-calling (predictive dialer) Android application built in Java. It allows automatic calling of a list of leads from a local array or Firebase database using the device's GSM SIM. The app includes features such as configurable call delays, call result logging, and CSV export options.

---

## 🔧 Features
- Auto-call using GSM SIM
- Configurable delay between calls (e.g., 10s, 30s)
- Call result tagging (Interested / Not Interested / Call Later)
- Simple button to start/stop auto-calling
- Offline support via local Room DB
- Firebase integration for syncing leads and logs (optional)
- CSV export to local storage

---

## 🛠 Project Structure
```
LeadCatchProApp/
├── app/
│   └── src/
│       └── main/
│           ├── java/com/askbharath/leadcatchpro/MainActivity.java
│           └── res/layout/activity_main.xml
├── build.gradle (project-level)
├── app/build.gradle (module-level)
├── settings.gradle
├── gradle/wrapper/gradle-wrapper.properties
└── google-services.json (optional)
```

---

## 🧱 Requirements
- Android Studio (Giraffe or above recommended)
- Android SDK 30+
- JDK 17 or 11
- USB-connected Android phone with a working SIM card

---

## ⚙️ Setup Instructions

1. Clone or extract the project in Android Studio.
2. Update gradle-wrapper.properties:
```
distributionUrl=https\://services.gradle.org/distributions/gradle-7.6-all.zip
```
3. In build.gradle (project), set:
```
classpath 'com.android.tools.build:gradle:7.0.4'
```
4. Sync project with Gradle files.
5. Clean + Rebuild the project.
6. Run the app on a connected Android device.

---

## 📞 Permissions
Add these to AndroidManifest.xml:
```xml
<uses-permission android:name="android.permission.CALL_PHONE" />
<uses-permission android:name="android.permission.INTERNET" />
```

---

## 🧪 Testing Steps
1. Open the app on your phone.
2. Tap "Start Auto Calling".
3. Calls will begin in sequence with a 10s delay.
4. Observe logs for debugging call state.

---

## 📤 Exporting Call Logs (optional)
The app can generate a CSV log of all calls including:
- Name
- Phone number
- Timestamp
- Result (Interested / Not Interested / Call Later)

---

## 🛠 Future Enhancements
- Lead import from Excel
- Voice recording (if legally allowed)
- Google Sheets sync
- Dashboard for analytics

---

## 🧑‍💻 Maintainer
Developed by: AskBharath & Team
Contact: gopigunaganti143@gmail.com

