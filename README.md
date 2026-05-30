# Chess Battle

Chess Battle is a native Android chess app designed for phones. It includes:

- A touch-friendly chess board with Unicode pieces and highlighted legal moves.
- Local multiplayer pass-and-play.
- Online room flow with shareable room codes, ready for connection to a backend endpoint.
- Bullet, blitz, rapid, and classic clock presets.
- Legal move validation, self-check prevention, check, checkmate, stalemate, promotion, undo, restart, resign, and time-loss handling.

## Build the APK

This repository is configured as a Gradle Android project. On a machine with Android SDK installed and network access for Gradle dependencies, run:

```bash
gradle :app:assembleDebug
```

The debug APK will be created at:

```text
app/build/outputs/apk/debug/app-debug.apk
```

Install it on a connected Android phone with:

```bash
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

> Note: the current execution environment blocks downloads from the Android/Gradle artifact repositories and does not include an Android SDK, so the APK cannot be produced inside this container. The project source is complete and ready to build where those Android tooling requirements are available.
