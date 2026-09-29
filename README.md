# Date Calculator (PWA)

Files:
- index.html      the whole app
- manifest.json   makes it installable
- sw.js           makes it work offline
- icons/          app icons

## Deploy free on GitHub Pages
1. Create a new public repo on GitHub, e.g. `date-calculator`.
2. Upload all files (keep the `icons` folder).
3. Repo Settings > Pages > Source: "Deploy from a branch" > branch `main`, folder `/ (root)` > Save.
4. After about a minute your app is live at:
   https://<your-username>.github.io/date-calculator/

## Install on phone
- Android (Chrome): menu > "Install app" or "Add to Home screen".
- iPhone (Safari): Share > "Add to Home Screen".

## When you change anything
Edit the file, then change `CACHE = "datecalc-v1"` in sw.js to `datecalc-v2`
so installed apps pick up the update.

## v2 additions
- Greeting with time of day ("Good evening") and your name, saved on the device.
- Live clock and date.
- Location and weather (Open-Meteo, free, no API key). Needs HTTPS, so it works
  after you deploy (GitHub Pages is HTTPS). Tap "Use my location" or "Search city".
- To change "Hai" to "Hi", edit `var HELLO = 'Hai';` in index.html.
