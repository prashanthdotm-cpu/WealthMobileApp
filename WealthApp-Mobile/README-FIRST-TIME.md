# WealthApp Mobile — first-time setup

## What is included
- Your existing app.js
- Your existing styles.css
- PWA manifest and service worker
- App icons
- Capacitor configuration for Android

## iPad PWA test
1. Upload the contents of `www/` to an HTTPS host such as GitHub Pages.
2. Open the HTTPS URL in Safari on iPad.
3. Use Share -> Add to Home Screen.
4. Launch WealthApp from the Home Screen.

## Android APK
The Android project must be compiled with the Android SDK/Gradle toolchain.
This package contains the Capacitor source configuration, but no precompiled APK is claimed to be ready.
On a computer with Node.js, Android Studio and the Android SDK:
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android

Then build/run from Android Studio. For a release APK, use Android Studio's Build APK(s) option.

## Important
The current app uses browser LocalStorage for local data. This is retained as-is for the first mobile/PWA test.
