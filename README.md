# REPS — My Gym Tracker

A mobile-first, zero-dependency gym planner and workout logger.

## Features

- Monday / Wednesday / Friday alternating Workout A and Workout B.
- Personalised machine workouts, a lower-volume comeback mode after a break, configurable sets/reps.
- Full ordered exercise walkthrough with last-used weights, individual set logging, and pause/skip rest countdown.
- Incline treadmill warm-up and post-workout cardio countdowns.
- History with previous weights and reps, workout duration, and optional weight/waist measurements.
- Offline-capable once loaded, installable to the home screen on supported browsers.
- Local browser storage, JSON export/import backups. **No account or cross-device sync**.

## Deploy with GitHub + Render

1. Create a new GitHub repository called `reps-gym-tracker` and upload these files to the root of the repository (not the ZIP archive itself).
2. At [Render](https://dashboard.render.com/static/new), select **New Static Site** and connect the repository.
3. Branch: `main`.
4. Build command: `echo "No build needed"`.
5. Publish directory: `.` (a dot).
6. Deploy. The site will be available at its Render URL with HTTPS and redeploy when the repo changes.

No environment variables or paid services are required. No build tooling is needed.

## Important notes

- Suggested weights are editable and are **historical reference values, not instructions** to lift those weights immediately after time away. Adjust for comfort and form.
- The app does not control the treadmill. Inclines/durations are suggestions, not medical recommendations.
- Previous session weights are offered as suggestions; all sets can be manually changed.
- If you clear the browser storage or use a different device/browser, your data won't appear without importing a backup.
- After updates, the service worker refreshes cached files when online. Close and reopen the app if you're still seeing an earlier version.

## Local test

Run `python3 -m http.server 8000` in this folder and visit http://localhost:8000.