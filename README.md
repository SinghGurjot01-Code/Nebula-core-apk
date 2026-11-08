# Nebula Android

Native Android customer app for the Nebula cloud-gaming platform.

## Build

The GitHub Actions workflow builds the Android project directly from the repository root.

1. Download the project ZIP from the project release shared with the maintainer.
2. Extract the ZIP contents into the repository root. The root must contain `settings.gradle.kts`, `build.gradle.kts`, and `app/build.gradle.kts`.
3. Commit and push the extracted files.
4. Open **Actions → Nebula Android APK**. The APK is uploaded as the `nebula-v0.0.3-debug-apk` artifact.

Do not upload the ZIP as a nested archive. The workflow expects the Android source tree at repository root.

## Current scope

- Kotlin + Jetpack Compose
- Light theme
- Local demo authentication, games, bookings, tickets and profile
- No wallet or admin dashboard
- Supabase authentication and live Moonlight streaming are future integrations, not active in this frontend-only build.

The workflow installs JDK 17, Android SDK 35 and Gradle 8.9 on GitHub-hosted runners. It does not require a checked-in Gradle wrapper.
