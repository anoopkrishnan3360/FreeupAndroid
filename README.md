# FreeUp (Android starter)
Copies old photos/videos to a drive folder, verifies size + SHA-256, then deletes originals via the system dialog.
No INTERNET permission, no accounts, no analytics.

## Build
1. Install Android Studio (latest). File > Open > this folder. Accept any Gradle/AGP upgrade prompts.
2. Change applicationId in app/build.gradle.kts to your own (e.g. com.yourname.freeup).
3. Add an icon: right-click app > New > Image Asset, then add android:icon in the manifest.
4. Test on a real phone with a USB drive/SD card.
5. Build > Generate Signed App Bundle (AAB). Create a keystore and BACK IT UP; enrol in Play App Signing.
6. Upload the .aab in Play Console (closed testing first).

## Not done yet
Google Play Billing (isPremium stub), foreground service for long copies, laptop Wi-Fi transfer,
app lock, resume after interruption, tests. Use the prompt pack in the guide to add these.
Play Console needs: privacy policy URL, Data Safety form, photo/video permission declaration.
