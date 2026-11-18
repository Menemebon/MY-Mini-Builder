📱 MY BUILDER
Code on Your Phone • Build APKs on Your Phone • Sign on Your Phone

An Android app development workshop for people without a PC.

✨ Features
🌐 Convert WEB / WEBSITE projects into signed APK files directly on your phone (no PC required).
🔑 Generate, import, export, and back up Keystores (.p12).
🎮 Ready-made mini-games: Snake, Memory, Balloon Pop, Jump, and Tic-Tac-Toe.
Play games directly.
Add games to your projects and build your own APK.
⚙️ Customize app icons, permissions, theme colors, fullscreen mode, and JavaScript bridge:
Android.toast
Android.share
Android.vibrate
Android.copy
Android.openUrl
📦 Export Java / Kotlin projects as Android Studio ZIP files.
🚀 Installation (One-Time Setup on PC)
Open Android Studio.
Select File > Open and choose this project folder.
Wait for Gradle Sync to finish.
If prompted, select Use JVM 21.
Select Build > Build APK(s).
Find the generated APK here:
text
app/build/outputs/apk/debug/app-debug.apk

Install the APK on your phone.

After this one-time setup, you can use My Builder directly on your phone.

📲 How to Use on Your Phone
Select New Project.
Choose WEB or WEBSITE.
Alternatively, go to Ready Games > Add to Project.
Write your code or enter a URL.
Tap Test to preview your project.
Tap Build APK.
Choose Install or Save / Share.
Updating Your App
You must use the same signing key when updating your application.
Go to Keys > Back Up to back up your keystore.
Keep your .p12 backup somewhere safe.
⚠️ Limitations
Java/Kotlin projects cannot be compiled directly on a phone.
Java/Kotlin projects can be exported as ZIP files and opened in Android Studio on a PC.
Generated APKs require Android 7.0 (API 24) or higher.
If you lose your keystore, you may not be able to publish updates to your existing app.

Always back up your keystore!

📁 Project Structure
text
app/
└── src/
    └── main/
        ├── java/
        │   └── com/
        │       └── mybuilder/
        │           └── app/       # Java application source code
        └── assets/
            ├── games/             # Ready-made HTML games
            └── template/          # ZIP export templates

🛠️ Built With
Java
Android SDK
Gradle
HTML / CSS / JavaScript

<p align="center">
Made with ❤️ by N.U.B STUDIO
<br>
<b>MY BUILDER</b>
</p>
