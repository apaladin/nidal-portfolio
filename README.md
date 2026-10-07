# Nidal Alsayyed: Portfolio

Static, single-page portfolio (plain HTML/CSS/JS, no build step).

## Edit content
All projects and apps are defined in the `PROJECTS` and `APPS` arrays near the bottom of `index.html`.
Categories (labels and colours) are in `CATEGORIES`. Stats are calculated from that data automatically.

Screenshots:
- `assets/shots/<slug>.webp`: desktop, full-length page capture at 1440px wide (saved at 1100px, up to ~4000px tall)
- `assets/shots/<slug>-m.webp`: mobile, full-length page capture at 390px wide (saved at 420px)
- On hover (or automatically on touch screens) each card scrolls through the whole captured page.
- `assets/apps/`: app icons and screens from the App Store listings

`<slug>` is the project domain without `www.`, with dots replaced by dashes (e.g. `toddsnyder-com`).
Set `featured: true` on a project to make its card span the full width. To keep the grid's last row full, make sure the number of non-featured projects is even.

## Run locally
Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy to Vercel
- **Dashboard:** push this repo to GitHub, then go to vercel.com/new, import it, keep Framework Preset = "Other", and deploy.
- **CLI:**

```bash
npx vercel --prod
```
