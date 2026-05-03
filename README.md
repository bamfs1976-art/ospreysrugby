# Ospreylia FanView

Unofficial Ospreys supporter companion — built by fans, for fans.

[![Netlify Drop deploy](https://img.shields.io/badge/deploy-Netlify%20Drop-2dd4bf)](https://app.netlify.com/drop)

## What it is

A single-file HTML web app for Ospreys rugby fans. Every screen is rendered locally — no external APIs, no build tooling, no frameworks. Drag the file to [drop.netlify.com](https://app.netlify.com/drop) and it's live.

> This is an unofficial fan site and is not associated with Ospreys Rugby, the URC or the WRU.

## Surfaces

| Page | Contents |
| --- | --- |
| **Home** | Next-match countdown, URC league position, last 5 form, season summary, history snapshot, legend spotlight |
| **Squad** | Senior squad placeholder (full Phase 2 data lives in `ospreys-rugby.html`) |
| **Fixtures** | 2025–26 fixtures, results with try scorers, full sortable URC standings |
| **History** | 7-era timeline + 23-season records table (2003–04 → 2025–26) |
| **Honours** | 4 league titles, Anglo-Welsh Cup 2008, Australia 2006, 21 Lions tourists |
| **Head-to-Head** | All-time records vs every opponent, Welsh derbies highlighted |
| **Analytics** | 6 inline-SVG charts — points, position, tries, win %, top scorers, top apps |
| **Coaches** | Every head coach 2003–present with tenure, win rate, trophies |
| **Venue** | Swansea.com Stadium + St Helen's + The Gnoll heritage |
| **Settings** | Dark/light theme, Welsh toggle, storage status |

## Stack

- **Single HTML file** — `ospreylia-fanview.html` (≈ 111 KB)
- **Vanilla JS, embedded CSS, embedded data** — no build step, no dependencies
- **`localStorage`** with safe-fallback wrapper for theme + language
- **CSP** locked to `'self'` — no third-party scripts, fonts or images
- **WCAG 2.2 AA** in both dark and light modes (orange `#F47920` ≥ 7.17:1 dark, `#A6480B` ≥ 5.57:1 light)

## File layout

The app is also published as `index.html` so it serves as the root document on Netlify / GitHub Pages.

```
ospreysrugby/
├── index.html              # entry point (= ospreylia-fanview.html)
├── ospreylia-fanview.html  # canonical filename
├── netlify.toml            # security headers
└── README.md
```

## Brand stance

- Original fan-safe SVG mark — shield silhouette + dual chevron feathers. **Not** the official Ospreys crest.
- Branded as "Ospreylia FanView" / "Built by fans, for fans" / "Unofficial Ospreys supporter companion".
- Welsh language toggle covers navigation and section headers.

## Data accuracy

All historic and current-season figures are flagged in-app where they are best-effort. Cross-reference against:

- [ospreysrugby.com](https://www.ospreysrugby.com)
- [unitedrugby.com](https://www.unitedrugby.com)
- [ultimaterugby.com](https://www.ultimaterugby.com)
- [espn.co.uk/rugby](https://www.espn.co.uk/rugby)

## Deploy

1. Drag `index.html` (or the whole folder) to [drop.netlify.com](https://app.netlify.com/drop).
2. That's it.

Or, for a custom Netlify site with the security headers from `netlify.toml`, link the GitHub repo and let Netlify build from `main`.

## License

The code is released for personal / non-commercial fan use. Ospreys, URC and WRU trademarks belong to their respective owners.
