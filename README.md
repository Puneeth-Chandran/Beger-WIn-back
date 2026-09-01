# Berger Paints — Contractor Win-Back Tracker

A field-first web app for tracking lost and at-risk contractors, logging follow-ups, and managing the win-back process.

**Built by:** Shreyas Krishna — MBA SIP 2026, Berger Paints India Limited, Prolinks Division, Thrissur Region

---

## Features

- 5-tier contractor segmentation (Tier 3 / 4 / 5 + Won Back)
- Add and edit contractor profiles with root cause, competitor, last product used
- Log every follow-up — phone call, site visit, WhatsApp, kit delivery, trial project
- Win-back progress bar: Not contacted → Contacted → Kit delivered → Trial → Won back
- Filter by tier or search by name, area, product, competitor
- Export to CSV
- Data saved in browser localStorage — no backend needed
- Fully responsive — works on mobile and desktop
- Dark mode support

---

## Deploy to Vercel (3 steps)

### Option A — Vercel CLI (fastest)

```bash
# 1. Install Vercel CLI (one time)
npm install -g vercel

# 2. Go into the project folder
cd berger-tracker

# 3. Deploy
vercel
```

Follow the prompts. Your app will be live at a URL like `berger-tracker.vercel.app`.

---

### Option B — Vercel Dashboard (no CLI)

1. Go to [github.com](https://github.com) and create a **new repository** (e.g. `berger-tracker`)
2. Upload all files from this folder into that repository
3. Go to [vercel.com](https://vercel.com) → **Add New Project**
4. Select your GitHub repository
5. Vercel will auto-detect the settings. Click **Deploy**
6. Your app is live — copy the URL and share it

---

### Option C — Drag and Drop (easiest, no GitHub)

1. Go to [vercel.com](https://vercel.com) → Log in
2. On the dashboard, drag and drop this entire `berger-tracker` folder
3. Vercel deploys it instantly — no setup needed

---

## Local development

```bash
# Install dependencies
npm install

# Run locally
npm run dev

# Build for production
npm run build
```

---

## Project structure

```
berger-tracker/
├── index.html        ← The entire app (HTML + CSS + JS)
├── package.json      ← Vite build config
├── vite.config.js    ← Vite settings
├── vercel.json       ← Vercel routing config
├── .gitignore
└── README.md
```

---

## Notes

- All data is stored in the browser's `localStorage` under the key `bp_winback_v2`
- Data persists across sessions on the same device and browser
- To share data across devices, use the CSV export and re-import manually (or contact the developer to add a cloud backend)
- The app works fully offline after first load

---

*Berger Paints India Limited · Prolinks Division · Thrissur Region · SIP 2026*
