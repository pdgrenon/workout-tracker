# 5×5 Barbell Tracker

A minimal, offline-capable workout tracker for 5×5 barbell training with automatic progressive overload. Built as a single HTML file with zero build tools — just open it in a browser.

## Features

- **Guided workouts** — Alternates between two sessions (A and B) built around five compound barbell movements: squat, bench press, barbell row, overhead press, and deadlift
- **Progressive overload** — Automatically increases weight by 5 lb after a successful session; deloads 10% after 3 consecutive failures on a lift
- **Rest timer** — 90-second countdown between sets with pause/skip controls
- **Weight adjustment** — Manually set working weights from the home screen without logging a workout
- **Workout swap** — Switch between Workout A and B for your next session
- **History log** — Reverse-chronological list of all past sessions with weights and set completion
- **Progress charts** — Line graphs for each lift showing weight over time
- **Data management** — Add historical workouts with custom dates and delete logged workouts with confirmation
- **Persistent storage** — All data saved to `localStorage` in your browser

## Program Structure

The tracker alternates between two workouts, each built around compound barbell lifts:

| Workout A | Workout B |
|---|---|
| Squat 5×5 | Squat 5×5 |
| Bench Press 5×5 | Overhead Press 5×5 |
| Barbell Row 5×5 | Deadlift 1×5 |

Train three days per week, alternating A and B. Complete all prescribed sets and reps, and the app adds weight to the bar for next time. Fail to complete your sets three sessions in a row on a given lift, and it automatically deloads so you can rebuild momentum.

## Usage

### Run locally

Download `index.html` and open it in any modern browser. That's it.

### Install as a phone app

1. Host the file anywhere (GitHub Pages, Netlify, or any static host)
2. Open the URL on your phone
3. Tap **Share → Add to Home Screen**
4. Launch it from your home screen like a native app

### GitHub Pages

1. Fork or clone this repository
2. Go to **Settings → Pages** and set the source to the `main` branch
3. Your tracker will be live at `https://<username>.github.io/<repo-name>/`

## Tech

- Vanilla HTML, CSS, and JavaScript — no frameworks, no build step
- [Chart.js](https://www.chartjs.org/) for progress charts (loaded from CDN)
- [Google Fonts](https://fonts.google.com/) for Outfit and JetBrains Mono typefaces
- Data stored in `localStorage` (stays in your browser, never leaves your device)

## License

[MIT](LICENSE)
