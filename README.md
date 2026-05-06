# Golf Focus Tracker

Single-page web app for tracking a 1–10 focus score per golf shot, across multiple golfers.

## Features

- Add multiple golfers; switch between them with a tap
- Log each shot with a focus score (1–10), optional club, hole #, and note
- Per-golfer stats: average focus, last-10 trend, best/worst, score distribution, and average by club
- Points system: every shot with focus **7+** earns 1 point worth **$0.25**
- "Tab" view shows every golfer's running points and dollar total
- Leaderboard sorted by average focus
- Data persists in `localStorage` (per device); JSON export for backup
- Installable as a PWA on iOS / Android home screens

## Running it

It's a single static HTML file with no build step.

- **Local:** open `index.html` in a browser, or run `python3 -m http.server` in this folder
- **GitHub Pages:** Settings → Pages → deploy from `main` branch, root folder

## Tweaking

Open `index.html` and look near the top of the `<script>` block:

```js
const POINT_THRESHOLD = 7;   // focus score needed to earn a point
const POINT_VALUE = 0.25;    // dollars per point
```
