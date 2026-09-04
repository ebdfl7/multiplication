# Multiplication Flash Cards

Interactive multiplication practice for facts **1×1 through 12×12**. Practice individual multipliers, grouped sets, or everything at once. Track progress, use a keypad or your voice, and deploy as a single static HTML page (GitHub Pages friendly).

## Features

- **Individual sets** — buttons for ×1 through ×12  
- **Group sets** — 2–5, 6–8, 9–12, and All (1–12)  
- **Progress tracking** — per-multiplier accuracy, saved in the browser (`localStorage`)  
- **Button colors** — muted blue by default; turn **green** (with ✓) when accuracy is ≥ 90%  
- **Options**
  - Randomize card order  
  - Double the number of cards  
  - Reset all progress  
- **Keypad** — 0–9, delete (⌫), and Enter  
- **Voice answers** — say the number (e.g. “thirty-six” or “36”); requires microphone permission  

## How to use

1. Open `multiplication-flashcards.html` in a modern browser (or visit your GitHub Pages URL).  
2. Optionally enable **Randomize** and/or **Double the number of cards**.  
3. Tap a blue set button to start practicing.  
4. Enter the product with the keypad or enable **Voice answer** and speak the number.  
5. Progress bars update as you answer; high accuracy turns a set green.  

## Files

| File | Description |
|------|-------------|
| `multiplication-flashcards.html` | Full app (React via CDN + Babel). Single file, no build step. |
| `README.md` | This file |

You can rename `multiplication-flashcards.html` to `index.html` so the repo root opens the app on GitHub Pages.

## Deploy on GitHub Pages

1. Create a new repository.  
2. Add `multiplication-flashcards.html` (optionally as `index.html`) and this `README.md`.  
3. Push to GitHub.  
4. **Settings → Pages** → Source: Deploy from a branch → choose `main` (or `docs` folder if you prefer).  
5. Open the site URL, e.g. `https://YOUR_USERNAME.github.io/REPO_NAME/`.  

No Node, npm, or backend required. The site must be served over **HTTPS** for microphone access (GitHub Pages provides HTTPS).

## Browser support

| Feature | Notes |
|--------|--------|
| Core UI, keypad, progress | All modern browsers |
| Voice answers | Best in **Safari** (iOS/macOS), **Chrome**, and **Edge** (Web Speech API). Limited or unavailable in Firefox. |
| Microphone | User must allow mic access when prompted |

## Progress data

Progress is stored only in the browser’s `localStorage` under the key `multFlashProgress`. It is **not** synced across devices. Use **Reset all progress** on the home screen to clear it.

## License

TBD
