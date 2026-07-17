# Icons of the Game · 2000–2026

A visual reference gallery of the greatest footballers of the modern era.

## What it is

A single-page website featuring 103 legendary players from 2000–2026. Click any card to see their career highlights, peak years, best club, and position details. Filter by position or search by name.

## Adding card images

Images live in the `/images` folder. To add a card for a player:

1. Name the file using the player's name in lowercase with underscores, e.g.:
   - `lionel_messi.png`
   - `cristiano_ronaldo.png`
   - `kylian_mbappe.png`
2. Drop it into the `/images` folder
3. Update the player entry in `index.html` — find the player in the `PLAYERS` array and set `"image_file": "filename.png"`

## Adding new players

In `index.html`, find the `PLAYERS` array and add a new object:

```json
{
  "name": "Player Name",
  "nationality": "Nationality",
  "position": "ST",
  "peak_years": "2018–2024",
  "best_club": "Club Name",
  "notes": "Career highlights and achievements",
  "image_file": null
}
```

Position codes: `GK` · `RB` · `LB` · `CB` · `DM` · `CM` · `AM` · `RW` · `LW` · `ST`

## Deploying to GitHub Pages

1. Push this folder to a GitHub repository
2. Go to Settings → Pages → Source → `main` branch, `/ (root)` folder
3. Save — your site will be live at `https://yourusername.github.io/repo-name`

## Structure

```
/
├── index.html      ← everything lives here (HTML + CSS + JS + data)
├── images/         ← card images (PNG)
│   ├── gianluigi_buffon.png
│   ├── iker_casillas.png
│   └── ...
└── README.md
```
