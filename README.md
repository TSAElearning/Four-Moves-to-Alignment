# Four Moves to Alignment

An interactive leadership training scenario (8–10 minutes) from **The Space of Agnes Elisa**.

Learners help the Northstar Services team resolve a performance conflict after an AI-enabled support platform launch slips. A Connect-Four-style board tracks progress toward alignment: every strong leadership choice drops a connection disc, and every weaker choice shows a likely consequence so the learner can reconsider. Four connected discs reveal the team's solution.

**Audience:** Leaders, HR and L&D teams, and managers guiding workforce change
**Learning goal:** Practice resolving a performance conflict by listening, using evidence, aligning priorities, and measuring results.

## Features

- Six storyboard scenes, four decision points, and a closing screen with a call to action
- Animated Connect-Four board: discs drop, bounce, and connect with a winning line
- Sound effects generated in the browser with the Web Audio API (clicks, dialogue pops, scene whoosh, disc drop and thud, correct chime, consequence tone, win fanfare). No audio files are needed.
- Optional **Narration** toggle that reads the script aloud with the browser's speech synthesis
- Inline SVG icons for every concept (diagnose, align, design, pilot, data, people, job aids)
- Brand palette (berry, pinks, grays, golds, greens) with **Roboto Slab** headings and **Roboto** body text
- Keyboard accessible, screen-reader announcements, reduced-motion support, and a responsive layout for phones

## Project structure

This repository is a single self-contained file:

```
index.html   The full course: page, styles, icons, sounds, and scenario logic
README.md    This file
```

## Run locally

Double-click `index.html` to open it in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Publish with GitHub Pages

1. Create a new repository on GitHub (for example `four-moves-to-alignment`).
2. Upload `index.html` and `README.md` (**Add file → Upload files**).
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
5. After a minute the course is live at `https://<your-username>.github.io/four-moves-to-alignment/`.

## Editing the content

All scenario text lives in `index.html`, inside the `window.COURSE = { ... }` block (search for `COURSE`). Each scene has `lines` (dialogue), `question`, `options` (mark the best move with `correct: true`; give the others a `consequence`), and `feedback`.

---

© The Space of Agnes Elisa · [agneselisa.net](https://agneselisa.net)
