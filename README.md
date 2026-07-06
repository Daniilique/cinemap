# 🗺️ CINEMAP

**A film for every country in the world.**

Think of those scratch-off travel maps people use to mark every country they've visited — this is that, but for movies. Pick one film to represent each country, star your favorite if you add more than one, and fill in your own personal map of world cinema.

**[→ Live site](https://daniilique.github.io/cinemap/)**

![CINEMAP preview](og-image.png)

## Features

- 🌍 **Interactive world map** — zoom, pan, and click any country to add a film
- 🔍 **Live search** — type a title and get real suggestions with posters, years, and directors (via Wikipedia and optional OMDb/IMDb data)
- ⭐ **Multiple films per country** — add as many as you want, star one as your favorite
- 🎬 **Two views** — the world map, or a Windows-8-style Live Tile grid showing every pick at a glance
- ☀️🌙 **Light and Noir themes**
- 🖼️ **Poster wall export** — download a composite image of everything you've picked
- ⬇️⬆️ **Backup/restore** — export and import your picks as a JSON file
- 🌐 **Multi-language search** — type in Russian, Japanese, or Spanish and it searches the matching Wikipedia edition automatically

## How it works

This is a single self-contained HTML file — no backend, no build step, no dependencies to install. Everything (the map, the styling, the logic) lives in `index.html` and runs entirely in your browser.

- **Your picks are stored locally in your browser** (`localStorage`), not on a server. They're yours, and they stay on your device unless you export them.
- **Live search/posters** need an internet connection, since they call the Wikipedia and OMDb APIs directly from the page.
- **OMDb is optional** — without an API key, search still works off Wikipedia alone; adding a free key (via the link in the app) unlocks real IMDb-sourced posters, directors, and ratings.

## Running it yourself

There's nothing to install. Either:
- Open `index.html` directly in any browser, or
- Fork this repo and enable GitHub Pages (Settings → Pages → Deploy from a branch → `main` → `/root`) to host your own copy

## Credits & licensing

- World map: [flekschas/simple-world-map](https://github.com/flekschas/simple-world-map), CC BY-SA 3.0
- Film data & posters: [Wikipedia](https://www.wikipedia.org/) and [OMDb API](https://www.omdbapi.com/) (OMDb/IMDb data is for personal, non-commercial use)

## Support this project

If you like it, there's a small donation link in the footer of the site. No pressure — just there if you want to.
