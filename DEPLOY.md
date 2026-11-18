# Deploy to Vercel

This folder is a static site (no build step). `vercel.json` sets Framework Preset to "Other", so the existing Next.js setting on the project does not matter.

1. Replace the contents of your repo (or the folder you deploy from) with the contents of this folder. Keep `.vercel/project.json` so `vercel --prod` stays linked to the `ashmitsinghportfolio` project.
2. Push, or run `vercel --prod`.
3. Vercel dashboard > Analytics > enable Web Analytics (the old site used it; the script tag is already in `index.html`).
4. Google Search Console verification file (`google331d3ca4a519db29.html`) is kept at the root.

If the build complains about a framework, set Settings > General > Framework Preset to "Other" and clear Build/Output overrides.

## Domain
Canonical, sitemap, share card and JSON-LD all use `https://www.ashmitsingh.page`. If your primary domain is the apex (`ashmitsingh.page`), find and replace `https://www.ashmitsingh.page` in `index.html`, `robots.txt` and `sitemap.xml`.

## Contents
- `index.html`: shell, transitions, routing (#vlsi, #robotics, #about, #projects), SEO and share-card tags
- `pages/`: home, home-m (phones), vlsi, robotics, about, projects
- `assets/`: fonts, portrait, React and runtime, all local
- `resume-vlsi.pdf`, `resume-robotics.pdf`, `og-image.png`, `apple-touch-icon.png`, `robots.txt`, `sitemap.xml`, `404.html`
