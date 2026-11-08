# Nebula Android

Native Android customer app for Nebula.

## Build and APK

The GitHub Actions workflow builds the project from the flattened source ZIP in the repository root.

1. Upload the supplied **nebula-android.zip** to the repository root.
2. Open **Actions → Nebula Android APK**.
3. Download the **nebula-debug-apk** artifact from a successful build.

The archive must contain these paths at its root:
- `settings.gradle.kts`
- `build.gradle.kts`
- `app/build.gradle.kts`

The workflow extracts the archive to `source/`, installs JDK 17, Android SDK 35 and Gradle 8.9, compiles Kotlin, builds the debug APK, then runs unit tests and uploads their report separately.

## Current scope

- Kotlin + Jetpack Compose, light theme
- Local demo authentication, games, bookings, tickets and profile
- No wallet or admin dashboard
- Supabase authentication/data and real Moonlight streaming are planned integrations, not active in this frontend-first build
- No real booking or cloud-gaming session is created by demo mode
