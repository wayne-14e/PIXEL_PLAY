# PIXEL_PLAY
### `// ARCADE BAY · PXL-9 WAYFARER`

Six free retro games aboard a stranded spaceship. Play cartridges, synthesize plasma, and bring the reactor back online.

`SYSTEM STATUS: ONLINE` · `CARTRIDGES: 6` · `COST: 0`

## ▶ Boot the arcade

Open [`index.html`](./index.html) in a browser, or serve the folder locally:

```bash
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). Serving over HTTP is recommended for cartridge scanning.

## Search engine indexing

The site publishes [`robots.txt`](./robots.txt) and [`sitemap.xml`](./sitemap.xml) for its homepage and six game pages. The canonical and social URLs use `https://pixel-play-beta.vercel.app`; if the production domain changes, update those URLs in the HTML pages and both files. Submit `https://pixel-play-beta.vercel.app/sitemap.xml` in Google Search Console to request indexing.

## 🕹 Cartridge bay

| Cartridge | Genre | Build |
|---|---|---|
| NEON_DINO | Runner | [`games/dino_3d`](./games/dino_3d/) |
| NEON_SERPENT | Arcade | [`games/neon_serpent`](./games/neon_serpent/) |
| NEON_STACK | Puzzle | [`games/neon_stack`](./games/neon_stack/) |
| PIXEL_DASH | Runner | [`games/pixel_dash`](./games/pixel_dash/) |
| SHADEBLADE | Fighter | [`games/shadeblade`](./games/shadeblade/) |
| VOIDSTRIKE_2088 | Shooter | [`games/voidstrike_2088`](./games/voidstrike_2088/) |

## ⚙ Add a cartridge

Put a game's HTML build in its `games/<id>/` folder, then update its `src` entry in `GAMES` in [`index.html`](./index.html). Launch it from the arcade library; games run in the bay's iframe. If a build is missing, use the built-in calibration sim.

Controls vary by game. The calibration sim supports mouse/touch and arrow keys or **A/D**.
