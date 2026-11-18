<h1 align="center">📱 My Mini Builder</h1>

<p align="center">
  <b>Build, sign and update Android apps — entirely from your phone.</b><br>
  No PC required.
</p>

<p align="center">
  <img alt="Platform" src="https://img.shields.io/badge/platform-Android%2024%2B-3DDC84?logo=android&logoColor=white">
  <img alt="Language" src="https://img.shields.io/badge/language-Java-orange">
  <img alt="Version" src="https://img.shields.io/badge/version-5.0-blue">
</p>

---

## ✨ Features

- 🌐 **Web projects to APK** — turn HTML / CSS / JS projects (or a website URL) into a signed APK directly on your phone.
- 🔑 **Keystore management** — create, import, export and back up signing keys (`.p12`).
- ⚙️ **App settings** — icon, permissions, theme color, full screen, screen orientation and a JavaScript bridge (`Android.toast`, `Android.share`, `Android.vibrate`, `Android.copy`, `Android.openUrl`).
- 📦 **Android Studio export** — export Java / Kotlin projects as a ZIP to open in Android Studio.
- 💾 **Backup & restore** — save all projects into one ZIP file and restore them on any device.
- 🔄 **Over-the-air updates** — the app checks GitHub Releases for a newer version, downloads the APK and starts the installer.
- 🌍 **Bilingual UI** — Turkish when the phone language is Turkish, English otherwise.

---

## 🚀 Building the app (once, on a PC)

1. Open **Android Studio** → **File › Open** → select this folder.
2. Wait for Gradle Sync to finish (accept *Use JVM 21* if asked).
3. Run **Build › Build APK(s)**.
4. The APK is generated at `app/build/outputs/apk/debug/app-debug.apk`.
5. Install it on your phone. Everything else happens on the phone.

---

## 📲 Using the app

1. Tap **New project** and choose **WEB** or **SITE**.
2. Write your code or enter a URL, then tap **Test**.
3. Tap **Build APK**, then **Install** or **Save / Share**.
4. For future updates to a published app, you must sign with the **same key** — back up your keystore under **Keys › Back up**.

---

## ⚙️ Settings

Settings are app-wide and live outside of any project. Open them with the gear icon on the project list.

- **Backup**
  - *Save backup (ZIP)* — saves all projects into a single file.
  - *Restore from backup* — adds the projects from a ZIP as new projects. Existing projects are never overwritten.
- **Update**
  - *Check for updates* — compares the installed version with the latest GitHub Release and installs the new APK if you confirm.

The app also checks for updates quietly each time it starts and only shows a prompt when a newer version exists.

---

## 🔄 How updates work

The app reads the latest release of this repository:

```
https://github.com/Menemebon/MY-Mini-Builder/releases/latest
```

1. Update `versionCode` and `versionName` in `app/build.gradle` (for example `versionCode 6` and `versionName "5.1"`).
2. On GitHub, go to **Releases › Draft a new release**.
3. Set the tag to match the version, for example `v5.1`.
4. Attach the **signed** APK file (`.apk`) and publish the release.

Phones will then offer the update. Important requirements:

- The new APK must be signed with the **same signing key** as the installed app. An APK signed with a different key cannot be installed over the existing one.
- The release tag must be a **higher version** than the installed version.
- Android asks for permission to install unknown apps the first time. Allow it and tap *Check for updates* again.

---

## ⚠️ Limitations

- Java and Kotlin projects are not compiled on the phone; export them as ZIP and open them in Android Studio.
- Generated APKs target Android 7.0+ (minSdk 24).
- If you lose your keystore, you cannot update an app you have already published. Back it up.
- The package name `com.mybuilder.app` is kept on purpose. Changing it would make existing installations impossible to update.

---

## 🧩 Project structure

```
app/src/main/java/com/mybuilder/app/
  ProjectsActivity.java        → main screen (project list)
  GlobalSettingsActivity.java  → app-wide settings (backup, updates)
  UpdateChecker.java           → GitHub Releases over-the-air updates
  Installer.java               → streamed APK installation via PackageInstaller
  Backup.java                  → all-projects ZIP backup and restore
  GitHubSync.java              → network helpers
  Lang.java                    → Turkish / English text table
app/src/main/assets/template/  → Android Studio ZIP export template
```

---

## 📄 License

No license has been specified yet.

---

<p align="center">Made with ❤️ — <b>My Mini Builder</b></p>
