
# 📱 MY BUILDER

### Code on Your Phone • Build APKs on Your Phone • Sign on Your Phone

**An Android app development workshop for people without a PC.**

---

## ✨ FEATURES

- 🌐 Convert WEB / WEBSITE projects into signed APK files directly on your phone.
- 🔑 Generate, import, export, and back up Keystores (.p12).
- 🎮 Ready-made mini-games:
  - Snake
  - Memory
  - Balloon Pop
  - Jump
  - Tic-Tac-Toe
- ⚙️ Customize:
  - App icons
  - Permissions
  - Theme colors
  - Fullscreen mode
  - JavaScript bridge (toast, share, vibrate, copy, openUrl)
- 📦 Export Java / Kotlin projects as Android Studio ZIP files.

---

## 🚀 INSTALLATION

**One-time setup on a PC**

1. Open Android Studio.
2. Select File → Open.
3. Choose the MY BUILDER project folder.
4. Wait for Gradle Sync to finish.
5. Select Use JVM 21 if prompted.
6. Select Build → Build APK(s).

Your APK will be located at:

```text
app/build/outputs/apk/debug/app-debug.apk
```

7. Install the APK on your phone.

After this setup, you can use MY BUILDER directly on your phone.

---

## 📲 HOW TO USE

1. Open MY BUILDER.
2. Select New Project.
3. Choose WEB or WEBSITE.
4. Write your code or enter a URL.
5. Tap Test.
6. Tap Build APK.
7. Install, save, or share your APK.

### Updating Your App

- Always use the same signing key when updating your app.
- Open Keys → Back Up.
- Keep your `.p12` keystore backup safe.

---

## ⚠️ LIMITATIONS

- Java/Kotlin projects cannot be compiled directly on a phone.
- Java/Kotlin projects can be exported as ZIP files for Android Studio.
- Generated APKs require Android 7.0 (API 24) or higher.
- Losing your keystore may prevent you from updating your existing app.

**Always back up your keystore!**

---

## 📁 PROJECT STRUCTURE

```text
app/
└── src/
    └── main/
        ├── java/
        │   └── com/
        │       └── mybuilder/
        │           └── app/
        │               └── Java source code
        │
        └── assets/
            ├── games/
            │   └── HTML games
            │
            └── template/
                └── ZIP templates
```

---

## 🛠️ BUILT WITH

- Java
- Android SDK
- Gradle
- HTML
- CSS
- JavaScript

---

<p align="center">
  Made with ❤️ by N.U.B STUDIO
  <br>
  <strong>MY BUILDER</strong>
</p>
