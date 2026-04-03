# plantie

`plantie` is an Android WebView app that bundles a local HTML, CSS, and JavaScript chatbot-style interface.

## Install

Open the project in Android Studio and sync Gradle, or use:

```bash
gradlew.bat assembleDebug
```

## Use

Install and run on an Android device or emulator.

## How It Works

- `MainActivity.java` loads `file:///android_asset/index.html`
- the UI and bot logic live in `assets/index.html`, `style.css`, and `script.js`
