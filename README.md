<h1 align="center">📱 My Mini Builder</h1>
<h3 align="center">Code on your phone • Build APKs on your phone • Sign on your phone</h3>

<p align="center"><b>An Android app workshop for people without a PC.</b></p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-7.0%2B-3DDC84?logo=android&logoColor=white" alt="Android 7.0+">
  <img src="https://img.shields.io/badge/Language-Java-orange" alt="Java">
  <img src="https://img.shields.io/badge/Version-4.0-blue" alt="v4.0">
</p>

---

## ✨ What does it do?

- 🌐 Turns **WEB** (HTML / CSS / JS) and **SITE** (URL) projects into signed **APKs** right on your **phone**, no computer needed
- ✍️ Built-in **code editor**: syntax highlighting, undo / redo, file manager
- ▶️ **Live test**: run your project inside the app before building the APK
- 🔑 **Keystore manager**: generate new keys, import them, view the password, back up as `.p12`
- ♻️ **Automatic backup**: projects and keys are backed up to `Downloads/MyBuilder`. They are restored even if you uninstall and reinstall the app
- ☕ Ready-to-open **ZIP** export for **Java / Kotlin** projects in Android Studio
- 🔄 **Update check** from Settings (GitHub releases)

## ⚙️ Project settings

| Setting | Description |
|---|---|
| App name, package name | In `com.name.app` format, validated |
| Version name / code | Auto-increment supported |
| Icon | Pick from gallery or use the default icon |
| Screen orientation | Auto, portrait, landscape, sensor |
| Appearance | Fullscreen, keep screen on, status bar color |
| SDK | Min SDK and target SDK (max 34) |
| Permissions | Internet, camera, microphone, location, storage, notifications, vibration, contacts, calls, SMS, Bluetooth and more |
| APK signing | Default key or your own |
| External links | Open external links in the browser for SITE projects |

### 🔌 JS bridge

If you enable it in settings, your WEB projects can access phone features from JavaScript:

```js
Android.toast("Hello!");            // short on-screen message
Android.share("Text to share");     // share sheet
Android.vibrate(200);               // vibrate (ms)
Android.copy("Copy to clipboard");  // copy to clipboard
Android.openUrl("https://...");     // open in browser
```

## 🚀 Setup (once, on a PC)

1. Open Android Studio → **File > Open** → select this folder
2. Wait for Gradle Sync to finish (if it asks for a JVM, pick 17 or higher)
3. **Build > Build APK(s)** → `app/build/outputs/apk/debug/app-debug.apk`
4. Install the APK on your phone. Everything after this happens on the phone.

> You can also download the ready-made APK from the [Releases](../../releases) page.

## 📲 Using it on your phone

1. **New Project** → choose WEB, SITE, Java or Kotlin
2. Edit your files with **Write Code** (enter the URL for SITE projects)
3. Preview live with **Test**
4. **Build APK** → **Install** or **Save / Share**
5. To update the same app later, use the same key → **Keys → Back up**

## ⚠️ Limitations

- Java / Kotlin projects can't be compiled on the phone; export the **Project ZIP** and build it in Android Studio
- Generated APKs are WebView-based, minSdk 24 and above
- If you lose your keystore you can't update your app, so always back it up

## 📁 Structure

```
app/src/main/java/com/mybuilder/app/   → app code (Java)
app/src/main/assets/template/          → Android Studio ZIP template
app/src/main/res/                      → icons and theme
```

## 🧱 Requirements

- Android 7.0 (API 24) or higher
- To build: Android Studio, JDK 17+, Gradle 8.7

---

<p align="center"><b>by N.U.B Studio</b></p>
