# Code Cadet: Galaxy Builder — PWA Bundle

A learning game for Ethan, built as a Progressive Web App.

## What's in this folder
- `index.html` — the entire app (HTML + CSS + JS in one file)
- `manifest.json` — PWA configuration (icons, name, theme color)
- `sw.js` — Service Worker (offline caching)
- `icon-*.png` — App icons in various sizes
- `apple-touch-icon.png` — iOS home screen icon

## Deploy to Netlify (5 minutes, free, no signup needed)

1. Go to https://app.netlify.com/drop
2. Drag this ENTIRE folder (the folder, not individual files) onto the upload area
3. Wait ~10 seconds. Netlify gives you a URL like `https://random-name-123.netlify.app`
4. Done. The app is live.

Optional after deploy:
- Click "Site settings" → rename the URL to something like `cadet-ethan.netlify.app`
- Or attach a custom domain (free with Cloudflare DNS)

## Add to iPad Home Screen

1. On iPad, open the Netlify URL in **Safari** (not Chrome)
2. Tap the **Share** button (square with arrow up)
3. Scroll down → **Add to Home Screen**
4. Make sure **"Open as Web App"** is ON (default in iOS 26+)
5. Tap Add

Now Ethan can tap the Pixel icon to launch the app full-screen. Progress is saved to localStorage and persists across launches.

## Updating the app
When you make changes (e.g. add new lessons):
1. Edit `index.html`
2. **Important:** bump the `CACHE_NAME` version in `sw.js` (e.g. `'code-cadet-v4.2'`)
3. Re-drag the folder to Netlify (same site updates)
4. Next time Ethan opens the app, it auto-fetches the new version

Without bumping the cache name, the old version stays cached and your changes won't show.

## Backup
Progress backs up to `Eudemon547@gmail.com` via the email backup feature inside the app. If localStorage ever gets cleared (rare, but possible), restore by pasting the backup email contents into Parent Dashboard → "PASTE EMAIL".

## Parent Dashboard access
- Tap the Code Cadet logo (top-left) 5 times quickly
- Password: `eric2026`

## Customizing
At the top of `index.html` find these constants:
```js
const PARENT_PASSWORD = 'eric2026';
const PARENT_EMAIL = 'Eudemon547@gmail.com';
const CADET_NAME = 'Ethan';
```

Change any of them to suit. After changes, re-deploy and bump `CACHE_NAME` in `sw.js`.
