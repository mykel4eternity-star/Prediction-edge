# Prediction Edge — Android app source

This is a lightweight, offline Android WebView app for the Prediction Edge calculator.

## Build an APK using GitHub (no Android Studio required)
1. Create a new GitHub repository.
2. Upload the contents of this ZIP into the repository (keep the `.github` folder).
3. Open **Actions** and run **Build Prediction Edge APK** (or push to `main`).
4. When the workflow finishes, open its run and download the `Prediction-Edge-debug-apk` artifact.
5. Extract the artifact ZIP; install `app-debug.apk` on your Android phone. If Android asks, allow installs from that source.

## Build locally
Install Android Studio / Android SDK and Gradle 8.9, then run:
`gradle assembleDebug`

APK output:
`app/build/outputs/apk/debug/app-debug.apk`

## Notes
- Calculator works offline.
- History is saved locally on the device using browser storage.
- Probability estimates are user-entered and not verified predictions.
- This is a debug APK build; it is suitable for personal testing, not Play Store release signing.
