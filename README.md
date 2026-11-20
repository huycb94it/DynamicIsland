# Dynamic Island Android — starter project

Native Kotlin Android project. Package: `com.huy.dynamicisland`.

## Current prototype
- Permission screen for overlay and notification access.
- Foreground service that hosts an Android application overlay.
- Animated pill preview with expandable spring-like transition and music/charging/notification demo states.
- Boot receiver attempts to restore the service after reboot when overlay permission remains granted.

## Build
Requires JDK 17+, Android SDK Platform 35, Android Build Tools, and Gradle 8.9+.

```bash
gradle assembleDebug
```
APK output: `app/build/outputs/apk/debug/app-debug.apk`.

## Important implementation status
This is a first runnable scaffold, not the finished full-feature release. The current pill is a visual/interaction prototype. Live media-session integration, real battery events, volume observation, call-state integration, notification rendering, drag positioning, persistent preferences, and device-specific soak testing remain to be implemented. Android may restrict background services and boot launches; no app can guarantee the OS will never terminate it.
