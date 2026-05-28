# jitesh.solutions

A retro Windows 98-style interactive portfolio built with React — complete with a functional desktop, draggable windows, a Start menu, and playable DOS games.

---

## Features

- **Desktop OS experience** — teal desktop, taskbar, Start button, and window management styled after Windows 98
- **Portfolio sections** — Home, About, Experience, Projects, and Contact, all inside draggable windows
- **Playable DOS games** — Doom, Digger, Scrabble, and Oregon Trail powered by [js-dos](https://js-dos.com/)
- **Music projects** — original tracks embedded directly in the portfolio
- **Retro typography** — MS Sans Serif, Millennium, and Terminal bitmap fonts for full authenticity

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | React (Create React App) |
| DOS emulation | js-dos / wdosbox (WebAssembly) |
| Fonts | MS Sans Serif, Millennium, Terminal (TTF) |
| Deployment | Static site (served under `/os/` path prefix) |

---

## Running Locally

```bash
# Must be served under /os/ for asset paths to resolve
mkdir -p /tmp/portfolio/os && cp -r . /tmp/portfolio/os/
cd /tmp/portfolio && python3 -m http.server 8080
```

Open `http://localhost:8080/os/` in your browser.

---

## Games

| Game | File |
|------|------|
| Doom | `doom.jsdos` |
| Digger | `digger.jsdos` |
| Scrabble | `scrabble.jsdos` |
| Oregon Trail | `trail.jsdos` |

Click any game icon on the desktop to launch it in a DOS emulator window.

---

## Contact

**Rachamadugu Jitesh** — [GitHub @jitesh523](https://github.com/jitesh523)

© 2025 Rachamadugu Jitesh
