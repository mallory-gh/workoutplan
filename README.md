# Gym Log

A mobile-first gym tracker for iPhone and iPad. Plain HTML, CSS and JavaScript in one page (`index.html`), with no build step. Your data is saved in the browser's localStorage, on each device separately.

## Features
- **Programs:** a 6-day rotation (Day A–F). Comes preloaded with *Push/Pull/Legs Block A*. You can create, duplicate, edit and activate programs, and set each one's start date and length in weeks.
- **Today:** shows the day mapped to today's weekday, or rest/cardio. You can also switch to "next day in rotation". Tap any day to train it instead.
- **Logging:** weight and reps for every set, with big +/- buttons. Tap a number to type it. Add or remove sets on the fly.
  - Set 1 starts at last session's weight, and each later set starts at the previous set's weight.
  - The keypad has an "Also apply to the remaining sets" toggle.
  - Each exercise shows a "Last time" line with the date and every set.
  - The weight step defaults to 2.5 lb. Tap the "±" chip on an exercise to change its step (1 / 2.5 / 5 / 10).
- **Exercise types:** weight × reps, bodyweight (with optional added weight), timed (seconds), and mobility (reps only).
- **Swaps:** swap any exercise for one session. Your past swaps appear as quick suggestions, and the swapped-in exercise shows its own Last time line.
- **Progress:** a chart of top-set weight or estimated 1RM over time, with personal bests marked. A trophy appears the moment you hit a PB.
- **History:** a calendar of workout, cardio and rest days, plus workouts per week and per month.
- **Backup:** export and import JSON, and export a CSV (date, exercise, set, weight, reps, …) that opens in Numbers or Excel.
- **Offline:** works without signal once it has loaded once.

## Hosting on GitHub Pages
1. Merge this branch into `main`, or pick this branch in step 2.
2. On GitHub, open the repo and go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**. Pick the branch and `/ (root)`, then **Save**.
3. After about a minute the site is live at `https://<your-username>.github.io/workoutplan/`.

## Installing on iPhone or iPad
1. Open the URL in **Safari**.
2. Tap **Share → Add to Home Screen → Add**.
3. Always open the app from that icon. The home-screen app keeps its data separate from the Safari tab, and iOS doesn't clear home-screen app data for inactivity the way it can for websites.
4. Each device keeps its own data. Use **Export / Import** in the Programs tab to back up or move data between devices.
