# Apex — Setup Studio

A local-first F1 25 game setup companion built with React and Vite. Includes 24 circuits, 10 team preference profiles, weather and track temperature, 20 adjustable settings, guided handling fixes, a saved setup garage, and JSON import/export.

## Run locally

```sh
npm install
npm run dev
```

Open the local URL printed by Vite. `npm run build` produces a static app in `dist`; `npm run preview` previews that build. `npm test` checks the recommendation engine and import validation.

Recommendations are transparent heuristics, not official, telemetry-backed or lap-time-validated setups. Team offsets represent experimental preferences. The app uses an F1 25-style setting model; verify compatibility with your game version. Handling changes preview their values and trade-offs, and can be undone. Context changes reset the setup, with a reminder to save first.

Setups are stored in browser local storage. Export JSON for durable backups or moving devices; import files through the studio or garage. There is no backend, account or AI service. JSON files are for this app and do not automatically load into the game. The interface works without external services; Google Fonts is optional and falls back to local sans-serif fonts.

General setup principles: [EA F1 25 setup guide](https://help.ea.com/en/articles/f1/f1-25/car-setups-guide/). Apex is an independent, unofficial companion.

Appearance and temperature preferences are available in the header and saved in this browser. Temperature units affect display only; exports and recommendations continue to use Celsius. The interface follows your system theme on first use.

