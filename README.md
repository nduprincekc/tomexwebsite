# TOMEX Website

Static, framework-free website for TOMEX — Group 10, TechyJaunt Sprint.

## Pages
- `index.html` — Home (Hero, About Us, Our Services)
- `login.html` — Login
- `onboarding.html` — Role selection (Farmer / Buyer / Cold Storage / Logistics)
- `marketplace.html` — Sample listings grid
- `contact.html` — Contact form

## Structure
```
tomex-site/
├── index.html
├── login.html
├── onboarding.html
├── marketplace.html
├── contact.html
├── css/style.css
├── js/script.js
├── images/            (hand-drawn SVG illustrations — no external image dependencies)
└── vercel.json
```

No build step, no dependencies — pure HTML/CSS/JS.

## Deploy to Vercel

**Option A — Vercel CLI (fastest):**
```bash
npm install -g vercel
cd tomex-site
vercel
```
Follow the prompts (link/create a project). Vercel auto-detects this as a static site.

**Option B — GitHub + Vercel dashboard:**
1. Push this folder to a GitHub repo.
2. Go to vercel.com → New Project → import the repo.
3. Framework preset: "Other" (or leave as detected). No build command needed, output directory is the repo root.
4. Deploy.

## Notes for the team

- All product photography is replaced with hand-drawn SVG illustrations (no stock photo licensing/copyright concerns, loads fast, no external image requests).
- Marketplace listings are static sample data in `marketplace.html`'s inline script — swap in a real API call once the Backend track's endpoints are live.
- Login/signup forms are frontend-only (no real auth wired up) — connect to the Backend track's auth endpoints when ready.
- Fonts load from Google Fonts CDN (Poppins, Inter, Playfair Display) — requires internet access at runtime, which Vercel-hosted sites have by default.
