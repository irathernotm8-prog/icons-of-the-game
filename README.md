# Icons of the Game

A visual gallery of the greatest footballers of all time.

## Adding card images

Drop a PNG into `/images`. Filename rules — **lowercase, underscores, no accents, no spaces**:

| Player | Filename |
|--------|----------|
| Lionel Messi | `lionel_messi.png` |
| Paolo Maldini | `paolo_maldini.png` |
| N'Golo Kanté | `ngolo_kante.png` |
| Zlatan Ibrahimović | `zlatan_ibrahimovic.png` |

Then find the player in the `PLAYERS` array in `index.html` and change `"image_file": null` to `"image_file": "filename.png"`.

## Adding players

Add to the `PLAYERS` array in `index.html`:

```json
{
  "name": "Player Name",
  "nationality": "Nationality",
  "position": "ST",
  "peak_years": "2010–2018",
  "best_club": "Club",
  "notes": "Career highlights",
  "image_file": null
}
```

**Position codes:** `GK` · `RB` · `LB` · `CB` · `DM` · `CM` · `AM` · `RW` · `LW` · `ST`

## GitHub Pages

Settings → Pages → Source: `main` branch, `/ (root)` folder → Save.
