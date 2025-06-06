
BUILD INSTRUCTIONS for Next Gen Developers
================================

AUTOMATIC APK GENERATION:
This repository automatically generates APK files using GitHub Actions.
Simply check the "Releases" page to download the latest APK - no manual building required!

MANUAL BUILD (if needed):
1. Download and extract this repository
2. Open Android Studio
3. Select "Open an existing Android Studio project"
4. Navigate to the extracted folder and select it
5. Wait for Gradle sync to complete
6. Click the "Run" button or Build > Build Bundle(s) / APK(s) > Build APK(s)

REQUIREMENTS:
- Android Studio 2022.3.1 or newer
- Android SDK API 21+ (Android 5.0+)
- Java 8 or newer

COMMAND LINE BUILD:
1. Navigate to project directory
2. Run: ./gradlew assembleDebug (for debug APK)
3. Run: ./gradlew assembleRelease (for release APK)
4. Find APK in: app/build/outputs/apk/

GITHUB ACTIONS:
This repository includes a GitHub Actions workflow that:
- Automatically builds APK files on every push
- Creates releases with downloadable APK files
- Handles all build dependencies and environment setup

CUSTOMIZATION:
- App icon: Replace files in app/src/main/res/mipmap/
- App name: Edit app/src/main/res/values/strings.xml
- Colors: Edit app/src/main/res/values/colors.xml
- Website URL: Edit MainActivity.java

The generated APK will be a fully functional Android app that displays your website in a WebView.