# TuneNow 🎵

A lightweight, responsive music player web app built with vanilla JavaScript — play, pause, seek, shuffle, and loop, with a focus on smooth, low-latency audio playback and fast search.

**Live demo:** https://tunenow.netlify.app/

## Features

- 🎧 Core playback controls — play, pause, seek, shuffle, loop
- 🔍 Debounced search for fast, low-lag track lookup
- ⚡ Lazy loading of assets to reduce initial load time
- 📱 Responsive UI, optimized for smooth performance across devices
- 🚀 Continuous deployment via GitHub Actions → Netlify on every push to `main`

## Tech Stack

- **Frontend:** JavaScript (ES6+), HTML5, CSS3
- **Deployment:** Netlify
- **CI/CD:** GitHub Actions

## Project Structure

```
TuneNow/
├── css/            # Stylesheets
├── resources/       # Static assets (audio, images, icons)
├── src/             # Application source (JS logic, player controls)
├── index.html        # Entry point
└── package.json
```

## Getting Started

Clone the repo and install dependencies:

```bash
git clone https://github.com/SHAHZIL14/TuneNow.git
cd TuneNow
npm install
```

Run locally:

```bash
npm start
```

Then open `http://localhost:<port>` in your browser.

## How It Works

- **Playback engine** — handles play/pause/seek/shuffle/loop state and syncs it with the UI in real time.
- **Search** — input is debounced to avoid firing a lookup on every keystroke, keeping the UI responsive while typing.
- **Asset loading** — track art and audio resources are lazy-loaded so the app boots quickly even with a larger library.

## Deployment

Every push to `main` triggers a GitHub Actions workflow that builds and deploys the app to Netlify automatically — no manual deploy steps required.

## Roadmap

- [ ] Playlist creation and persistence
- [ ] Keyboard shortcuts for playback controls
- [ ] Dark mode
- [ ] Offline/PWA support

## Author

**Mohd Shazil Raza**
[GitHub](https://github.com/SHAHZIL14) · [LinkedIn](https://linkedin.com/in/shazilr)
