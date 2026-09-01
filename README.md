# FitPath 🏃‍♂️

A self-contained, zero-budget fitness web app — single HTML file, no backend required.

## Features
- **BMI Calculator** – personalized action plans and workout schedules
- **Workout Tracker** – logging with streak tracking
- **Exercise Calendar** – visual workout history
- **Diet Plans** – vegetarian & non-vegetarian meal plans with macro/micronutrient breakdowns
- **AI Coach** – powered by OpenRouter's free-tier models

## Tech Stack
- Vanilla HTML/CSS/JS, single file
- `localStorage` for data persistence
- OpenRouter API (`openrouter/free`) for AI coaching
- Apache Cordova for optional Android packaging

## Run locally
Just open `index.html` in a browser. No build step, no install.

## Set up the AI Coach
The app does **not** ship with an API key baked in — you add your own, and it's
stored only in your browser's `localStorage`, never in this repo.

1. Get a free key at [openrouter.ai/keys](https://openrouter.ai/keys) (no credit card needed)
2. Open the app → go to the AI Coach tab
3. Paste your key into the **"Save Key"** field and click Save

## Live Demo
👉 https://YOUR_USERNAME.github.io/fitpath/

## Build the Android APK (optional)
```bash
npm install -g cordova
cordova platform add android
cordova build android
```
Requires Temurin JDK 17 with `JAVA_HOME` set.

## Security note
Never commit an API key into `index.html`. This app is designed so keys stay
client-side in `localStorage` — keep it that way in any fork/edit.

## License
MIT
