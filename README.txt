Luxy AI - Made by Afraz Studio

FILES
index.html            The whole app (open in Chrome to test)
manifest.json         App name, colors, icons
icon-192.png          App icon (small)
icon-512.png          App icon (main, use for Android launcher)
icon-maskable-512.png App icon for adaptive/round Android icons

HOW TO USE
1. Create a GitHub repo and upload ALL files in this folder (keep them together).
2. Test first: open index.html in Chrome with internet on.
3. Build the APK with Capacitor or PWABuilder.

INTERNET PERMISSION (needed for online features)
- Capacitor: open android/app/src/main/AndroidManifest.xml and make sure this
  line is above the <application tag (Capacitor usually adds it for you):
    <uses-permission android:name="android.permission.INTERNET" />
- PWABuilder or other online APK builders add it automatically.

WEATHER
- Easiest: open the app, tap Settings, type your city in "Your city (for weather)", Save.
- Optional automatic location: also add
    <uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />

OPTIONAL SETTINGS (inside the app)
- Daily update URL: link to a config.json in your repo, for example
  {"system":"extra instructions for the AI","notice":"Message shown on the home screen"}
- Gemini key: optional, for better answers and reading pictures.
