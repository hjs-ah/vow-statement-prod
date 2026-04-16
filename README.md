# VOW Center — Giving Statement Portal

A clean, session-only giving statement generator for Verity Outreach Worship Center.

## Features

- **Form fields**: Patron name, email address, fiscal year, and amount given
- **Generate PDF**: Downloads a professionally formatted giving statement (jsPDF — runs entirely in the browser)
- **Email Summary**: Opens the user's default mail client pre-filled with the giving summary
- **Privacy-first**: No data is stored, transmitted, or persisted beyond the browser session
- **Session disclosure**: Privacy notice is visible on the form

## Deploy to Vercel (Recommended — 1 minute)

### Option A — Vercel CLI
```bash
npm i -g vercel
cd vow-giving-statement
vercel
```
Follow the prompts. Select "No" for build overrides — it's static.

### Option B — Vercel Dashboard (no CLI needed)
1. Zip the contents of this folder (NOT the folder itself — select `index.html`, `vercel.json`, `vow-logo.png`)
2. Go to [vercel.com](https://vercel.com) → New Project → Deploy
3. Drag and drop the zip file
4. Click Deploy — live in ~30 seconds

### Option C — GitHub + Vercel (auto-deploy on push)
1. Push this folder as a GitHub repo
2. Connect the repo in Vercel dashboard
3. Every push to `main` auto-deploys

## Local Preview
Just open `index.html` directly in a browser — no server needed.

## Notes
- PDF generation uses [jsPDF](https://github.com/parallax/jsPDF) loaded from CDN (no build step required)
- Email uses `mailto:` links — opens the user's default mail client. No SMTP or server required.
- The logo (`vow-logo.png`) must be in the same directory as `index.html`

## Files
```
vow-giving-statement/
├── index.html       # Complete app (HTML + CSS + JS)
├── vow-logo.png     # VOW Center logo (white/transparent)
├── vercel.json      # Vercel static site config
└── README.md        # This file
```
