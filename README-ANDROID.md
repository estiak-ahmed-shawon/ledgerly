# Ledgerly Android app (installable PWA)

This package turns Ledgerly into an installable Progressive Web App (PWA). On Android, it can be added to the home screen and opened in an app-like full-screen window. It is not an APK file.

## Important: a shareable phone link needs HTTPS hosting
Android Chrome generally requires an HTTPS website (or localhost) to install a PWA. You can test the app locally on your computer, but to open a link on your phone you need to publish this folder to a static HTTPS host such as GitHub Pages or Netlify.

## Quick install on Android
1. Publish the contents of this folder to a static HTTPS site.
2. Open the published URL in Chrome on your Android phone.
3. Open Chrome's menu (⋮) and tap **Install app** or **Add to Home screen**.
4. Confirm. Ledgerly will appear on your home screen and open in its own app-like window.

## Publish using GitHub Pages (free option)
1. Sign in to GitHub and create a new repository, e.g. `ledgerly`.
2. Upload all files and folders in this package (including `icons/`) to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under the build/deployment section, choose deployment from the `main` branch and `/ (root)`, then save.
5. Wait for GitHub Pages to publish. The URL will look like `https://YOUR-USERNAME.github.io/ledgerly/`.
6. Open that URL on Android Chrome and install it as above.

## Data and privacy
- Your records remain in the local storage of each browser/device; they do not sync automatically between your PC and phone.
- Export a JSON backup from Settings & backup and manually restore it on the other device if needed.
- The app has no login or cloud database. Do not store sensitive financial information on a shared device.
- Currency conversion rates are sample values and must be updated manually.
- Recurring schedules are tracked but are not automatically posted.

## Files
- `index.html`: Ledgerly application
- `manifest.webmanifest`: installable app metadata
- `service-worker.js`: offline caching support
- `icons/`: Android launcher icons
