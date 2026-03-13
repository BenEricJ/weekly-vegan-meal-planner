#  Weekly Vegan Meal Planner

A PWA (Progressive Web App) for creating weekly vegan meal plans  optimised for individual goals, budget, training and nutritional needs.

**Live URL:** https://benericj.github.io/weekly-vegan-meal-planner

---

## Install on iPhone

1. Open the URL in **Safari**: `https://benericj.github.io/weekly-vegan-meal-planner`
2. Tap the **Share button ()** at the bottom
3. Select **"Add to Home Screen"**

The app will behave like a native app  with its own icon, fullscreen mode and offline support.

---

## Android App

The project includes a native Android project (Capacitor). To open it in Android Studio:

```bash
npx cap open android
```

After making changes to `src/index.html`, sync first:

```bash
npx cap sync android
```

---

## Deploying Changes

After every change to the app (`src/index.html`, `src/sw.js`, etc.), GitHub Pages deploys automatically:

```powershell
cd "c:\Users\JoachiE\OneDrive - BASF\Python Projects\Weekly Vegan Meal Planner\weekly-vegan-meal-planner"
git add .
git commit -m "Update"
git push
```

GitHub Actions will deploy within ~30 seconds.

---

## Project Structure

```
src/
 index.html       # Main app (fully self-contained)
 manifest.json    # PWA manifest (icon, name, fullscreen)
 sw.js            # Service Worker (offline support)
 icons/           # App icons (192px, 512px)
 css/
    styles.css
 js/
     app.js
.github/
 workflows/
     deploy.yml   # Automatic GitHub Pages deployment
```

---

## Local Development Server

```powershell
$env:PATH = "C:\Program Files\nodejs;" + $env:PATH
npx serve src -l 3000
#  http://localhost:3000
```
