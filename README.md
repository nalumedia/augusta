# 2026 Masters — Best-4-of-6 Pool Predictor

Interactive single-file HTML tool for picking a 6-player team for a "best 4 of 6" Masters pool.

## Features

- Vegas-calibrated base scoring model (de-vigged outright odds → projected 72-hole scores)
- 10,000-iteration Monte Carlo simulator for any 6-player team
- Brute-force optimizer over C(18,6) combos under current conditions
- Historical backtest against the last 7 Masters (2019–2025)
- Augusta-specific adjustments: course fit, age curve, LIV rust penalty, weather scenarios
- SG:APP trend visualization (last 12 weeks) per player
- Weather sensitivity bars (Normal / Soft-Calm / Firm-Windy)
- Baseline vs adjusted-optimal comparison
- Shareable URLs (`?picks=0,1,2,3,4,5&w=firm`) and copy-as-text export

## Run locally

Open `index.html` in any modern browser. All math runs client-side with no server, no API calls, no build step.

## Deploy

Any static host works — GitHub Pages, Netlify, Cloudflare Pages, or just double-click the file.
