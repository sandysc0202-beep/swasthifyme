# SwasthifyMe

Indian diet, macro, water and weight tracker that runs entirely in the browser, in English and Hindi.

- 180 Indian foods with Hindi and Marathi names: fruits, dry fruits, fish, dals, sabzi, Maharashtrian dishes and Diwali faral
- Type what you ate ("2 roti, dal aur chaas", "नाश्त्याला पोहे आणि चहा") and log it in one tap; voice input where the browser supports it
- Search that understands everyday spellings (pohe, poli, anda, chiken) and ranks foods by your own habits, diet and region
- One-tap "usual meals", "same as yesterday", favourites and suggestions on every meal
- Calories, protein, carbs, fat, fiber and water per day, with a ±10% "on track" band instead of red failure states
- Streaks with freezes, 8 achievements, a daily coaching tip, weekly budget, month calendar and a 7-day-average weight trend
- Light, dark (OLED charcoal) and system themes; metric or imperial units; vegetarian, eggetarian, non-vegetarian or vegan; North, South, East and West food regions
- Onboarding that sets your targets in under a minute, with Asian-Indian BMI cut-offs and safe calorie floors
- Undo for every change, swipe to delete, autosaving goals
- Data stays in the browser's local storage; backup and restore as JSON
- Installable app (PWA) that works fully offline on phone and desktop

Nutrition values are approximate per serving. SwasthifyMe gives general estimates, not medical advice.

## Run it
Enable GitHub Pages (Settings → Pages → Deploy from branch → `main` / root), then open the Pages link.
Opening `index.html` straight from disk works too, but install and offline mode need it served over https or localhost.

## Install
- **Chrome / Edge on a computer:** click the install icon in the address bar, or the **Install app** button on the Me page.
- **Android:** Chrome menu → *Add to Home screen* / *Install app*.
- **iPhone:** Safari → Share → *Add to Home Screen*. This also stops Safari clearing your data after 7 days without a visit.

## Updating
After changing `index.html`, `foods.js` or the icons, bump `VERSION` in `sw.js` so installed copies pick up the new build.
Saved data from earlier versions (`swasthifyme_v1_state`, `swasthifyme_v2_state`) is migrated automatically.

## Files
- `index.html` — the app: design tokens, screens, logging, search, parser, streaks and insights
- `foods.js` — the food database, Hindi names, regions, egg foods and search spellings
- `manifest.json` — app name, colours, icons and the "Log food" shortcut
- `sw.js` — service worker that caches the app, food data and fonts for offline use
- `icons/` — app icons (standard, maskable and Apple)
