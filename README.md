# MetaHomeworkHelper

iOS app that connects to Ray-Ban Meta glasses, streams camera video, and captures homework photos via voice commands.

## Setup

1. Open `MetaHomeworkHelper.xcodeproj` in Xcode
2. The Meta Wearables DAT SDK SPM dependency is already configured. If Xcode doesn't resolve it automatically, go to **File > Packages > Resolve Package Versions**. The repository URL is: `https://github.com/facebook/meta-wearables-dat-ios`
3. Replace the `MetaAppID` value `0` in `Info.plist` with your real Meta App ID from the [Meta Developer Portal](https://developers.facebook.com/)
4. Select a physical iOS device as the build target (the DAT SDK requires real hardware)
5. Build and run

## Usage

1. **Connect** — Tap "Connect Glasses" to register your Ray-Ban Meta glasses via the Meta AI companion app
2. **Start** — Tap "Start" to begin the camera stream and voice listener
3. **Trigger** — Say "help me with my homework" to capture a photo of what the glasses see
4. **Instruct** — Speak your follow-up instructions (e.g., "solve problem 3")
5. **Review** — After 5 seconds of silence, the captured photo and your transcribed instructions are displayed

## Requirements

- iOS 17.0+
- Xcode 15.4+
- Physical iOS device
- Ray-Ban Meta glasses paired via Meta AI app
- Meta Developer App ID with DAT access enabled
