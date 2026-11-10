WA Lite - WebView wrapper around WhatsApp Web (Android 5+, tested target: Android 10)

OPTION A - Android Studio (easiest)
 1. Install Android Studio. File > Open > select this folder. Let Gradle sync.
 2. Build > Build APK(s). Output: app/build/outputs/apk/debug/app-debug.apk
 3. Copy to phone, open it, allow "install unknown apps".

OPTION B - No install, GitHub Actions
 1. Create a GitHub repo, upload this folder (including .github).
 2. Actions tab > "Build APK" > Run workflow. Download "WALite-apk" artifact (a zip containing app-debug.apk).

OPTION C - Command line (needs JDK 17, Android SDK, Gradle 8.7)
 gradle assembleDebug

First run: open the app, on your main phone go to WhatsApp > Linked devices > Link a device,
scan the QR code (or use "Link with phone number").
