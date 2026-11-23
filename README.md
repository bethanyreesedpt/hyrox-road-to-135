# HYROX Road to 1:35 — iPhone app

This is an installable Progressive Web App (PWA). It stores workout entries locally in the browser on the device.

## Included
- Strength, running, HYROX station/class, and knee-health logs
- History search and type filters
- Running distance, selected-lift load, and knee symptom charts
- Race countdown with editable race date
- JSON backup/restore and CSV export
- Home Screen install and basic offline app shell

## Important data note
Entries are saved in browser local storage on the device. They are not automatically synced to iCloud, another device, or ChatGPT. Export JSON backups regularly. If Safari website data is cleared, local entries may be lost. Use the JSON restore feature to recover a backup.

## Publish it so you can install it on iPhone
The app needs to be hosted at an HTTPS address for the PWA install and service worker to work. The simplest route:
1. Create a free GitHub account if you don't already have one.
2. Create a new public repository, e.g. `hyrox-road-to-135`.
3. Upload all files in this folder to the repository root.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish the site. It will show a URL like `https://YOUR-USERNAME.github.io/hyrox-road-to-135/`.
7. On your iPhone, open that URL in Safari, tap Share → Add to Home Screen → Add.
8. Open the new Home Screen icon. Add a test entry, close and reopen the app to verify it remains.

If you want a private URL or automatic cross-device sync, this local-only version is not sufficient; it would need an authenticated backend/database. Do not put sensitive personal information into a public repository.

## Updating
Replace the app files in the repository when you want to publish an updated version. Export a JSON backup before updates or changing devices.
