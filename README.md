# Nebula Android

Native Android customer app for Nebula.

## Build and download the APK

The source is stored as 11 binary Git objects under `source-chunks/`. GitHub Actions reconstructs the original XZ archive, verifies its SHA-256 checksum, extracts the Android project and builds it.

1. Open **Actions → Nebula Android APK**.
2. Open the latest successful run.
3. Download the `nebula-debug-apk` artifact.

The workflow uses JDK 17, Android SDK 35 and Gradle 8.9. It builds a debug APK without signing secrets.

## Current scope

- Kotlin + Jetpack Compose, light theme
- Local demo authentication, games, bookings, tickets and profile
- No wallet or admin dashboard
- Supabase authentication/data and real Moonlight streaming are planned integrations, not active in this frontend-first build
- Demo booking and authentication data remain local; no real gaming session is created
