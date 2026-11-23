# Streakline

A habit tracker that shows your year as a GitHub-style contribution heatmap. Add habits, check them off daily, and watch your streak grow.

Built with plain HTML, CSS and JavaScript. No framework, no build step, no backend.

## Features

- Year-long heatmap, darker squares for days when more habits were completed
- Per-habit current streak and best streak
- Overall stats: done today, longest streak, total check-ins
- Data saved in your browser (`localStorage`), nothing leaves your device
- Export your data as JSON
- Light and dark theme that follow your system setting
- Keyboard accessible, responsive down to mobile

## Run it

```bash
git clone https://github.com/<your-username>/streakline.git
cd streakline
open index.html   # or just double-click the file
```

## Deploy on GitHub Pages

1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set the source to the `main` branch, root folder
4. Your site goes live at `https://<your-username>.github.io/streakline/`

## How streaks work

A streak counts consecutive days with a check-in. If you haven't checked in yet today, yesterday's streak stays alive until the day ends.

## Data format

```json
{
  "habits": [
    { "id": "lx3k9", "name": "Push a commit", "days": ["2026-11-21", "2026-11-22"] }
  ]
}
```

## Roadmap

- [ ] Import from JSON
- [ ] Weekly goals per habit
- [ ] Per-habit heatmap view

## License

MIT
