# 🗺️ CINEMAP

**A film for every country in the world.**

Think of those scratch-off travel maps people use to mark every country they've visited — this is that, but for movies. Pick one film to represent each country, add as many as you want, star your favorite to show it on the map, and fill in your own personal map of world cinema.

**[→ Live site](https://daniilique.github.io/cinemap/)**

![CINEMAP preview](og-image.png)

## Features

- 🌍 **Interactive world map** — zoom, pan, and click any country to add a film
- ⚡ **Instant, verified search** — a bundled local database of ~250,000 films (via TMDB) makes search work offline and instantly, and since it includes each film's real production countries, results show whether a match is actually confirmed for that country — not just a title-text guess
- 🎲 **Surprise me** — don't have a film in mind? Get a random, genuinely verified pick for the selected country
- ✍️ **Add anything custom** — can't find something in search (obscure, personal, or fan-made)? Add it manually with your own title, year, director, and poster link
- ⭐ **Multiple films per country** — add as many as you want, star one as your favorite to show on the map and list
- 🎬 **Two views** — the world map, or a tile grid showing every pick at a glance, including a Live-Tile-style flip animation between poster and details
- ☀️🌙 **Light and Noir themes**
- 🖼️ **Poster wall export** — download a composite image of everything you've picked, with country name and flag on each tile
- ⬇️⬆️ **Backup/restore** — export and import your picks as a JSON file
- 🌐 **Multi-language search** — type in Russian, Japanese, Spanish, or one of eight Indian scripts (Hindi, Bengali, Tamil, Telugu, and more) and it automatically searches the matching Wikipedia edition
- 🏳️ **A couple of deliberate flag choices** — Belarus and Russia show the historical/opposition flags (white-red-white and white-blue-white) instead of the current official state flags

## How it works

This is a single self-contained HTML file plus one data file — no backend, no build step, no dependencies to install.

- **The local film database** (`movies.jsonl.gz`) is fetched once when the app loads and decompressed natively in your browser. It's what makes search instant and lets country matches be genuinely verified rather than guessed.
- **Your picks are stored locally in your browser** (`localStorage`), not on a server. They're yours, and they stay on your device unless you export them.
- **Posters/directors for anything outside the local database** — or as a fallback — come from Wikipedia (no key needed) or OMDb (optional free key, unlocks real IMDb-sourced data). This part needs an internet connection.

## Running it yourself

There's nothing to install. Either:
- Open `index.html` directly in any browser (with `movies.jsonl.gz` sitting in the same folder), or
- Fork this repo and enable GitHub Pages (Settings → Pages → Deploy from a branch → `main` → `/root`) to host your own copy

## Credits & licensing

- World map: [flekschas/simple-world-map](https://github.com/flekschas/simple-world-map), CC BY-SA 3.0
- Film search database: [TMDB](https://www.themoviedb.org/) — this product uses the TMDB API but is not endorsed or certified by TMDB
- Additional film data & posters: [Wikipedia](https://www.wikipedia.org/) and [OMDb API](https://www.omdbapi.com/) (OMDb/IMDb data is for personal, non-commercial use)

## Support this project

If you like it, there's a small donation link in the footer of the site. No pressure — just there if you want to.
