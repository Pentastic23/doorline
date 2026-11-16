# Doorline

A door-to-door sales tracker for reps in the field. It runs in the phone's browser and can be installed to the home screen.

- **Today:** daily goal ring, a doors → talked → pitched → closed funnel, comparison with your 7-day average, doors by hour, and follow-ups due today.
- **Territory:** a live map that follows your GPS position. Every door is a pin colored by its result, and you can tap any spot on the map to log a door there. A street-by-street list is also available.
- **Log door:** fills in the address from your GPS position. One tap records the outcome (Not home, Not interested, Callback, Interested, Sale or Do not knock). "Save & next door" moves you to the next house on the same side of the street.
- **Follow-ups:** overdue, today and upcoming callbacks, plus a searchable pipeline.
- **Team:** a leaderboard by sales, revenue or doors, and a 14-day trend.
- Works offline. Data is stored on the device and can be exported as a CSV from Settings.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app (HTML, CSS, JS) |
| `leaflet.js`, `leaflet.css` | Leaflet 1.9.4 map library, bundled locally for offline use |
| `manifest.webmanifest`, `icon*` | Lets you install the app to the home screen |
| `sw.js` | Service worker for offline use |
| `claude-preview.html` | The claude.ai preview version, which has team sync but no map |

Map tiles © OpenStreetMap contributors © CARTO. Address lookup by OpenStreetMap Nominatim.

The app needs HTTPS for GPS, which GitHub Pages provides. To run it locally, use `python3 -m http.server` and open `http://localhost:8000`.
