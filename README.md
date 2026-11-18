
📱 MY BUILDER
Code on Your Phone • Build APKs on Your Phone • Sign on Your Phone

An Android app development workshop for people without a PC.

✨ What Does It Do?
🌐 Converts WEB / WEBSITE projects into signed APK files directly on your phone (no PC required).
🔑 Generates, imports, exports, and backs up Keystores (.p12).
🎮 Ready-to-play mini-games: Snake, Memory, Balloon Pop, Jump, Tic-Tac-Toe — play them or add them to your project and build your own APK.
⚙️ Customize app icons, permissions, theme colors, fullscreen mode, and JavaScript bridge (Android.toast / share / vibrate / copy / openUrl).
📦 Exports Java / Kotlin projects as Android Studio ZIP files.
🚀 Installation (One-Time Setup on a PC)
Open Android Studio → File > Open → Select this folder.
Wait for Gradle Sync to finish (if prompted, select Use JVM 21).
Select Build > Build APK(s) → Find the APK at app/build/outputs/apk/debug/app-debug.apk.
Install the APK on your phone. From this point on, everything can be done directly on your phone.
📲 How to Use on Your Phone
Select New Project → Choose WEB or WEBSITE (or go to Ready Games → Add to Project).
Write your code or enter a URL → Tap Test.
Tap Build APK → Install or Save / Share.
To update your app, you must use the same signing key → Go to Keys → Back Up.
⚠️ Limitations
Java/Kotlin projects cannot be compiled directly on your phone (export as ZIP → build with Android Studio).
Generated APKs require minSdk 24 or higher.
If you lose your keystore, you won't be able to publish updates to your app. Always keep a backup!
📁 Project Structure
text
app/src/main/java/com/mybuilder/app/   → Application source code (Java)
app/src/main/assets/games/             → Ready-made games (HTML)
app/src/main/assets/template/          → ZIP export templates


<p align="center">Made with N.U.B STUDIO — <b>My Builder</b></p>
