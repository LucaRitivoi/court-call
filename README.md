Court Call 🎾

Live app: https://LucaRitivoi.github.io/court-call/

A weather-based tool that tells you whether tennis courts are actually safe and dry enough to play on right now — tailored to the surface, because a hard court, clay court, and grass court all dry and get slippery in completely different ways.

What it does
Search any location (or use your device's location) to pull live weather.
Pick a surface — hard, clay, or grass — and get a playability score built specifically around how that surface behaves in rain, humidity, and wind.
Pinpoint your exact court on an interactive map, since weather is regional but conditions can still vary slightly by exact spot.
Save courts you play at often for quick one-tap switching.
Sun & glare timing — calculates the sun's position throughout the day and flags hours where it sits low on the horizon (a real hazard for players facing into it).
Estimated dry-by time — a rough projection of when a wet court should be playable again, factoring surface type, rainfall, wind, humidity, and sunset.
5-day forecast with the same surface-specific scoring, so you can plan ahead.
Why the scoring is strict

Playability is deliberately conservative — this isn't "would I risk it," it's closer to tournament-standard: active rain always caps the score low regardless of anything else, and courts don't count as dry again just because the rain stopped a few minutes ago.

How it's built

A single self-contained HTML file — no backend, no build step, no server. It runs entirely in the browser and pulls data from:

Open-Meteo — free weather + geocoding APIs (no key required)
Leaflet.js + OpenStreetMap — the interactive map
SunCalc — sun position and sunrise/sunset math

Because it has no backend, saved courts are session-only and reset when you close the tab.

Running it locally

Just download index.html and open it in any browser — no installation needed. To deploy your own copy, this repo is already set up for GitHub Pages (Settings → Pages → deploy from main branch, root folder).

Disclaimer

This is a weather-based estimate. It doesn't know an individual court's drainage, shade, or maintenance history — always trust what you see on-site over the score.
