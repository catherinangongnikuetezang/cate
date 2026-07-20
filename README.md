# Catherina Ngongni Kuetezang — Personal Website

A single-page, fully static personal site (no build step, no dependencies) ready for **GitHub Pages**.

```
.
├── index.html                 ← the whole site
├── assets/
│   ├── img/                    ← optimised photos
│   └── doc/Catherina-Kuetezang-CV.pdf
└── README.md
```

## Deploy to GitHub Pages (5 minutes)

**Option A — user site (nicest URL: `catherina.github.io`)**
1. Create a new repository named exactly **`<your-username>.github.io`**.
2. Upload every file here, keeping the folder structure (`index.html` must sit at the repository root).
3. Go to **Settings → Pages**, set **Source = Deploy from a branch**, **Branch = `main` / `root`**, Save.
4. Wait ~1 minute. The site is live at `https://<your-username>.github.io`.

**Option B — project site (URL: `<username>.github.io/<repo>`)**
1. Create any repo, e.g. `personal-website`, and upload these files.
2. **Settings → Pages → Deploy from a branch → `main` / `root`**.
3. Live at `https://<username>.github.io/personal-website`.

### From the command line
```bash
git init
git add .
git commit -m "Launch personal website"
git branch -M main
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main
# then enable Pages in Settings → Pages
```

## Editing
- All text lives in `index.html` — search for a phrase and edit it in place.
- Swap a photo by replacing the file in `assets/img/` (keep the same filename), or point the `src` at a new one.
- Colours and fonts are CSS variables at the top of the `<style>` block (`:root { --ink … --gold … }`).
- The résumé button links to `assets/doc/Catherina-Kuetezang-CV.pdf` — replace that file to update it.

## Notes
- Fonts load from Google Fonts; everything else is local, so the site works offline once cached.
- A phone number was intentionally **left off** the public page to reduce scraping; add it in the contact section if wanted.
- Custom domain: add a `CNAME` file with your domain and configure DNS per GitHub's docs.
