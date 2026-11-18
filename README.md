📱 My Mini Builder

<p align="center">
<b>Build, Sign & Update Android Apps — Directly From Your Phone!</b>
<br>
No PC required for everyday app building.
</p>

<p align="center">
<img src="https://img.shields.io/badge/Platform-Android%207.0%2B-3DDC84?logo=android&logoColor=white">
<img src="https://img.shields.io/badge/Language-Java-orange?logo=java">
<img src="https://img.shields.io/badge/Version-5.0-blue">
<img src="https://img.shields.io/badge/Status-Active-success">
</p>

🚀 Download

<p align="center">
<a href="https://github.com/Menemebon/MY-Mini-Builder/releases/latest">
<img src="https://img.shields.io/badge/⬇%20DOWNLOAD%20APK-Latest%20Release-2ea44f?style=for-the-badge">
</a>
</p>

Download the latest APK from GitHub Releases:

👉 https://github.com/Menemebon/MY-Mini-Builder/releases/latest

Always get the latest available version.
Download the APK directly to your Android device.
Install it and start building apps!
✨ Features
🌐 Web to APK
Convert HTML, CSS and JavaScript projects into Android APKs.
Turn existing websites into Android applications.
Preview projects before building.
Generate signed APK files directly on your phone.
🔑 Keystore Manager
Create signing keys.
Import existing keystores.
Export and back up .p12 files.
Keep your signing keys safe for future updates.
⚙️ Advanced App Settings

Customize your applications with:

Custom app icons.
Android permissions.
Custom theme colors.
Full-screen mode.
Screen orientation.
JavaScript bridge support.

Available JavaScript functions:

Android.toast
Android.share
Android.vibrate
Android.copy
Android.openUrl
📦 Android Studio Export
Export Java and Kotlin projects as ZIP files.
Open exported projects in Android Studio.
Continue development on a computer.
💾 Backup & Restore
Back up all projects into one ZIP file.
Restore projects on another device.
Existing projects are never overwritten.
🔄 Automatic Updates
Check GitHub Releases for new versions.
Download newer APK versions.
Start Android's package installer.
Get update notifications when a new version is available.
🌍 Languages
English interface.
Turkish interface.
Automatic language selection based on device language.
🛠️ Build From Source

You only need a PC once to build the application.

Install Android Studio.
Open this repository using File → Open.
Wait for Gradle Sync.
Use JDK 21 if requested.
Select Build → Build APK(s).
Find the generated APK here:

app/build/outputs/apk/debug/app-debug.apk

Install the APK on your Android device.

After installation, you can create and build web applications directly from your phone.

📲 How to Use
Open My Mini Builder.
Tap New Project.
Choose WEB or SITE.
Write your HTML, CSS and JavaScript code or enter a website URL.
Tap Test to preview your application.
Tap Build APK.
Install, save or share your generated APK.

Important: Always back up your signing key. Future updates to an already published application must use the same signing key.

🔄 Publishing Updates on GitHub

My Mini Builder uses GitHub Releases to distribute new versions.

To publish an update:

Open app/build.gradle.
Increase versionCode and update versionName.
Build and sign the new APK.
Open your GitHub repository.
Navigate to Releases → Draft a new release.
Create a new tag, such as v5.1.
Upload the signed APK.
Publish the release.

Your users can download the new version from:

https://github.com/Menemebon/MY-Mini-Builder/releases/latest

Update Requirements
The APK must use the same signing key as the previously installed version.
The new version must have a higher versionCode.
Android may request permission to install apps from unknown sources.
Never lose your original signing key.
📱 System Requirements
Requirement	Details
Operating System	Android 7.0 Nougat or newer
Minimum SDK	API 24
Programming Language	Java
Build System	Gradle
Java Version	JDK 21 for building

What is Android API 24?

API 24 corresponds to Android 7.0 Nougat. This means the app supports Android 7.0 and newer versions, not Android version 24.

⚠️ Limitations
Java and Kotlin projects cannot be compiled directly on the phone.
Java and Kotlin projects can be exported as ZIP files for Android Studio.
Generated applications require Android 7.0 or newer.
Losing your signing key prevents normal updates to applications signed with that key.
The package name com.mybuilder.app is intentionally preserved for compatibility with existing installations.
📂 Project Structure
text
app/src/main/java/com/mybuilder/app/
├── ProjectsActivity.java
├── GlobalSettingsActivity.java
├── UpdateChecker.java
├── Installer.java
├── Backup.java
├── GitHubSync.java
└── Lang.java

app/src/main/assets/template/
└── Android Studio ZIP export template

📄 License

No license has been specified yet.

<p align="center">
<b>Made with N.U.B STUDİO</b>
<br>
My Mini Builder
<br><br>
<a href="https://github.com/Menemebon/MY-Mini-Builder/releases/latest">
Download Latest Version
</a>
</p>
