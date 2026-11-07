# SwasthifyMe

Indian diet, macro, water and weight tracker that runs entirely in the browser.

- 180 Indian foods with Marathi/regional names: fruits, dry fruits, fish, dals, sabzi, Maharashtrian dishes and Diwali faral
- Calories, protein, carbs, fat, fiber and water per day
- Weight log, 7-day trends, BMI (Asian-Indian cut-offs), BMR and maintenance calories
- Custom dishes, edit/move logged items, repeat yesterday's meals
- Data stays in the browser's local storage; backup and restore as JSON
- Installable app (PWA) that works fully offline on phone and desktop

Nutrition values are approximate per serving.

## Run it
Enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root), then open the Pages link.
Opening `index.html` straight from disk works too, but install and offline mode need it served over https or localhost.

## Install
- **Chrome / Edge on a computer:** click the install icon in the address bar, or the **Install app** button in the sidebar.
- **Android:** Chrome menu → *Add to Home screen* / *Install app*.
- **iPhone:** Safari → Share → *Add to Home Screen*.

## Updating
After changing `index.html` or the icons, bump `VERSION` in `sw.js` so installed copies pick up the new build.

## Files
- `index.html` — the whole app
- `manifest.json` — app name, colours and icons for installing
- `sw.js` — service worker that caches the app and fonts for offline use
- `icons/` — app icons (standard, maskable and Apple)
