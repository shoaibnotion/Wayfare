# Wayfare – Holiday Planner

A mobile-friendly holiday planner built as a single-page HTML app.

## Files
- `index.html` — the app (original app logic retained, with app icon/PWA metadata and service-worker registration added)
- `manifest.json` — installable web-app metadata
- `service-worker.js` — basic app-shell offline caching
- `icons/` — app icons and browser favicon

## Publish with GitHub Pages
1. Create or open a **public** GitHub repository.
2. Upload the **contents** of this folder, keeping the `icons` folder intact.
3. Make sure `index.html` is in the repository root.
4. Open **Settings → Pages**.
5. Under Build and deployment, choose **Deploy from a branch**.
6. Select branch `main` and folder `/(root)`, then Save.
7. Wait for deployment and open the URL shown in GitHub Pages.

## Install on Android
1. Open the published HTTPS website in Chrome.
2. Open the three-dot menu.
3. Choose **Install app** or **Add to Home screen** if offered.

## Important data behaviour
Wayfare currently stores trips, packing lists, reminders, photos and notes in the browser's local storage on that device/browser. It does not have accounts or cloud synchronization. Different users have separate data. Clearing browser storage can remove locally saved data, so users should keep their device/browser data safe.

The service worker provides basic offline caching after the first successful online visit. Browser notifications are subject to browser permission and platform restrictions; scheduled reminders are checked while the app is open, not by a background push service.
