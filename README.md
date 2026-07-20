# Icons of the Game · 2000–2026

A visual gallery of the 120 greatest footballers of the modern era.

## Adding card images

All images go in `/images`. Name the file using lowercase and underscores — no accents, no spaces:

| Player | Filename |
|--------|----------|
| Cristiano Ronaldo | `cristiano_ronaldo.png` |
| Kylian Mbappé | `kylian_mbappe.png` |
| Lionel Messi | `lionel_messi.png` |
| N'Golo Kanté | `ngolo_kante.png` |

**Rules:**
- Lowercase only
- Spaces → underscores
- Strip accents (é→e, ö→o, ü→u, etc.)
- Strip apostrophes and dots
- PNG format

Once you drop the file in, find the player in the `PLAYERS` array inside `index.html` and update their `"image_file"` field from `null` to `"filename.png"`.

## Adding new players

Find the `PLAYERS` array in `index.html` and add:

```json
{
  "name": "Player Name",
  "nationality": "Nationality",
  "position": "ST",
  "peak_years": "2018–2024",
  "best_club": "Club Name",
  "notes": "Career highlights",
  "image_file": null
}
```

**Position codes:** `GK` · `RB` · `LB` · `CB` · `DM` · `CM` · `AM` · `RW` · `LW` · `ST`

## Deploy to GitHub Pages

1. Push repo to GitHub
2. Settings → Pages → Source: `main` branch, `/ (root)`
3. Live at `https://yourusername.github.io/repo-name`

## File structure

```
/
├── index.html        ← entire site (HTML + CSS + JS + data)
├── images/           ← card PNGs (transparent background works best)
└── README.md
```
