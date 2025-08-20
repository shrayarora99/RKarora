
# Estate Empire — Static Site (Navy/White)

This package is a deploy‑ready website for your private consultancy.

## How to deploy (no coding)

### Option A — Netlify (recommended for forms)
1. Go to https://app.netlify.com/ → **Add new site** → **Deploy site**.
2. Drag & drop the entire `estate-empire-site` folder.
3. Forms work out of the box (Netlify Forms). Submissions live in **Netlify → Forms**.

### Option B — Vercel / GitHub Pages
- Site will deploy, but the forms won’t collect by default.
- If you want forms on Vercel, replace `data-netlify="true"` with a Formspree endpoint:
  - Create a free Formspree project → get your endpoint (e.g. `https://formspree.io/f/xxxxxx`).
  - In `buyers.html` and `owners.html`, set `action` to that URL and **remove** `data-netlify`/hidden `form-name`.

## Customize
- Replace WhatsApp number and email in `contact.html`.
- Logo is at `/assets/logo.png` and favicon `/favicon.png`.
- Colors are configured via Tailwind in `<head>` (navy/royal/muted).

## Privacy
All forms are private. We never display phone or email publicly.
