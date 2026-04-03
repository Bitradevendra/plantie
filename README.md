# plantie

`plantie` is an Android WebView application that packages a local HTML, CSS, and JavaScript chatbot-style interface.

## Overview

The Android shell loads bundled web assets from the app package and presents them inside a native WebView.

## Project Structure

```text
plantie/
|-- app/
|   `-- src/main/
|       |-- assets/
|       |-- java/
|       `-- res/
|-- gradle/
|-- build.gradle.kts
`-- README.md
```

## Requirements

- Android Studio
- Android SDK

## Installation

Open the project in Android Studio and let Gradle sync, or build from the command line:

```bash
gradlew.bat assembleDebug
```

## Running The Project

Install the debug build on a device or emulator:

```bash
gradlew.bat installDebug
```

Then launch the app from the device.

## How It Works

- `MainActivity.java` loads `file:///android_asset/index.html`.
- `assets/index.html`, `style.css`, and `script.js` define the chatbot UI and behavior.
- Android resources under `res/` provide the native wrapper styling and launcher assets.
