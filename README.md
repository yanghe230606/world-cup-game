# World Cup Cheer Penalty

A browser-based World Cup penalty shootout game. Players choose a national team, take penalty shots, and build fan power on the leaderboard.

## Features

- 48 selectable teams with flag assets
- Penalty shootout interaction with goalkeeper animations
- Fan power leaderboard and result screen
- Optional camera gesture control powered by MediaPipe
- Static HTML, CSS, and JavaScript. No build step is required.

## Project Structure

```text
.
├── index.html          # Main game page
├── app.js              # Game logic
├── styles.css          # Visual styles and layout
├── image/              # Game art, flags, court, players, and UI assets
├── docs/               # Notes and standalone animation previews
├── .gitignore
├── .gitattributes
└── README.md
```

## Run Locally

You can open `index.html` directly in a browser for a quick preview.

For camera gesture control, run the project from a local web server so the browser can grant camera access:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## GitHub Pages

This project can be published directly with GitHub Pages:

1. Push the repository to GitHub.
2. Open the repository settings.
3. Enable Pages from the main branch.
4. Use `/` as the publish folder.

## Notes

- The game uses local image assets under `image/`.
- Camera gesture detection loads MediaPipe files from public CDN URLs when enabled.
- Keep filenames and folders unchanged unless you also update their references in `index.html`, `styles.css`, and `app.js`.
- Asset source and attribution notes are documented in `CREDITS.md`.
