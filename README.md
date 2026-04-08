# Plantie

A lightweight Android WebView app that wraps a bundled chatbot-style web interface inside a native mobile shell.

## Why It Stands Out

`plantie` is small, but it has charm: it takes a local HTML, CSS, and JavaScript experience and turns it into something that feels app-like on Android without needing a backend.

## What It Does

- loads local web assets through Android WebView
- packages the chat UI as an installable Android project
- keeps interaction self-contained inside the app

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

Open the project in Android Studio and let Gradle sync, or build with:

```bash
gradlew.bat assembleDebug
```

## Run Locally

Install the debug build on a device or emulator:

```bash
gradlew.bat installDebug
```

## How It Works

- `MainActivity.java` opens `file:///android_asset/index.html` inside a WebView.
- `assets/` contains the actual chatbot page, styling, and script logic.
- Android resources in `res/` provide the surrounding mobile shell.

## Best Fit

This project is great when you want to package a web interaction as a quick Android app without rebuilding the experience natively.
