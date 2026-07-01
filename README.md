# NeuroTouch

**Hands-free Android phone control for people with mobility disabilities.**

NeuroTouch uses your phone's front camera to track your head movements and eye blinks — no touching the screen required. Move your head to move a cursor, blink both eyes to tap.

> **Draft / Early Version** — this is a work in progress. Expect rough edges.

## How it works

| Action | What to do |
|---|---|
| Move cursor | Tilt / turn your head |
| Tap | Blink both eyes simultaneously |
| Recalibrate | Press the Calibrate button in the app |

You can also switch between **Head Pose** and **Eye Gaze** tracking modes, and adjust cursor sensitivity from the main screen.

## Requirements

- Android 7.0 (API 24) or higher
- Front-facing camera
- Android Studio (to build from source — no APK available yet)

## Build & Install

1. Clone or download this repository
2. Open the `NeuroTouch2` folder in **Android Studio**
3. Connect your Android device via USB (enable USB Debugging in Developer Options)
4. Click **Run** (the green play button)

## Setup (first launch)

Grant all three permissions when prompted — the app won't work without them:

1. **Camera** — needed to see your face
2. **Display over other apps** — needed to show the cursor overlay
3. **Accessibility Service** — needed to perform taps on your behalf
   - Go to Settings → Accessibility → find **NeuroTouch** → enable it

Then press **Calibrate** while looking straight at the camera. The cursor will snap to center and start tracking.

## Tech stack

- Kotlin / Android
- ML Kit Face Detection (head pose + eye openness)
- CameraX
- Android Accessibility Service (gesture dispatch)
## Team

Built by **SONIC_HUB** — Nazarbayev Intellectual School, Astana, Kazakhstan
