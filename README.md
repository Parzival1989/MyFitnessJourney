# MyFitnessJourney

A responsive, accessible, **single-file** daily meal tracker based on a five-meal printed plan. No framework, backend, database, accounts, analytics, or external dependencies.

## Get started

1. Download `index.html` and open it in a modern browser, or serve it from any static web host (GitHub Pages works well).
2. Select the day, mark meals eaten, and choose breakfast/protein/starch alternatives.
3. Optionally record water, weight, additional foods and daily notes.
4. Use **Export JSON** regularly; **Import JSON** on another browser/device to restore the data. Imports *replace* the current history after confirmation.

## Privacy and persistence

All tracking data lives in your browser's `localStorage` under `myfitnessjourney:v1`. It survives normal reloads and browser restarts, but **does not automatically sync across devices**, and can be lost if you clear site data, use private browsing, or change the site's origin. JSON backups are intentionally user-controlled. If you open `index.html` as a `file://` URL, browser storage behavior may differ by browser; a static site host provides a stable origin.

Do not commit your exported personal-health JSON files into a public repository. The repo should contain only the app source.

## Features

- Five meal checkoffs per day, alternative options, portions transcribed from the original document
- Daily completion ring, full-day streak and interactive seven-day chart
- Water tracker (8-glass visual reference, adjustable count up to 30)
- Optional weight, extra-food log, and free-form notes
- One-click date navigation
- Automatic browser persistence; import/export JSON backups
- Keyboard-accessible controls, responsive layout, reduced-motion support
- Fully usable offline once the HTML file is available

## What this is not

The original handwritten calorie/macronutrient annotations were ambiguous and vary by food choice. This app deliberately does not claim accurate calorie or macro totals. A meal checkoff is self-reported and not a substitute for nutrition advice. The water target is a visual tracker, not an individualized hydration prescription.

## Optional GitHub Pages hosting

Repository **Settings → Pages → Deploy from a branch → `main` / root**. The URL will typically be `https://<username>.github.io/MyFitnessJourney/`. The app source may be publicly visible if the repo is public, but your locally stored tracking data will not be uploaded to GitHub by the app.

## Project layout

- `index.html` — app, styling and JavaScript (the only runtime file)
- `README.md` — instructions and data handling notes
- `.gitignore` — prevents backup files from being accidentally committed