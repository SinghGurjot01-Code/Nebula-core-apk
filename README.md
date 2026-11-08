# Nebula Android

Native Android frontend project for Nebula.

## Build APK

1. Download the corrected `nebula-android.zip` from the project handoff and upload it to the repository root with the exact filename `nebula-android.zip`.
2. Push the file to `main` (or run **Actions → Nebula Android APK → Run workflow** after uploading).
3. Open the **Actions** tab, select the latest **Nebula Android APK** run, and download the `nebula-v0.0.2-debug-apk` artifact.

The workflow extracts the project, installs JDK 17, Android SDK 35 and Gradle 8.9, compiles Kotlin, builds the debug APK, runs unit tests and uploads the APK plus test report.

## Current scope

Frontend/demo phase only. Authentication, bookings, tickets and profile data are local demo implementations. Google/Supabase authentication and real Moonlight/Sunshine streaming are not connected yet.
