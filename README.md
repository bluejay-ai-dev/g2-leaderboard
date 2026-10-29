# G2 voice agent leaderboard

Static site for the G2 × Bluejay voice AI agent platform evaluation: the leaderboard, one page per platform and the methodology, with the two PDF reports.

Live at https://g2-leaderboard-production.up.railway.app/

## Files

| Path | What it is |
|---|---|
| `index.html` | Leaderboard: scores, Pareto frontiers, reliability |
| `provider-*.html` | One page per platform |
| `methodology.html` | Full methodology |
| `methodology.css` | Stylesheet for every page |
| `css/`, `media/`, `g2-assets/`, `brand/`, `logos/` | G2 site styles, fonts and logos |
| `reports/` | Methodology and scorecard PDFs |

## Run locally

```bash
python3 -m http.server 8742
```

## Deploy

Railway project `g2-leaderboard`, service `g2-leaderboard`. Caddy serves the folder as is.

```bash
railway up --service g2-leaderboard --detach
```
