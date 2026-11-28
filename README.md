# thenoblehouse.com

One static page served by GitHub Pages from the `main` branch root.

- `index.html`: the whole page. One screen, no scrolling. The harbour sketch draws in from the bottom up (canvas), then the name, tagline, rule and contact fade in.
- `assets/sketch-desktop.webp` / `assets/sketch-mobile.webp`: the background sketches (fine charcoal lines + 30% gold wash, transparent sky over the teal page colour). The mobile one is used when the screen is taller than 5:4.
- `assets/wear.webp`: the worn-ink texture masked over all text and the red rule.
- Compass (top): a heading tape the width of the name, drawn on `#tape`. It works out where the visitor is from their browser timezone (the `TZ` table in `index.html`, IANA zone → reference city, built from tzdata; no network call), then shows the great-circle bearing and distance to Miami Beach in leagues (1 league = 3 nautical miles). It fades in on north, swings and settles on the heading (~3 s), then drifts slightly. Hidden if the timezone isn't in the table (e.g. UTC) or JS is off; settled with no motion for reduced-motion users.
- Colours: red `#E73D46`, teal `#4CD1CE`, gold `#D4AF5A`, ink `#1E2627`.

Edit `index.html` directly and push to `main`.
