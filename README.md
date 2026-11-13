# Vikas Kumar – Portfolio

A single-page portfolio built with plain HTML, CSS and JavaScript. No build step, no dependencies.

## Structure
```
portfolio/
├── index.html
├── css/style.css
├── js/script.js
├── assets/images/   (profile.jpg, favicon.svg, og-image.png)
├── assets/documents/resume.pdf
└── README.md
```

## Test locally
1. Quick: double-click `index.html`.
2. Better: in the `portfolio` folder run `python -m http.server 8000`, then open http://localhost:8000.

## Add or change things
- **Photo:** replace `assets/images/profile.jpg` (keep the name, or edit the `<img>` in the hero).
- **Resume:** replace `assets/documents/resume.pdf` with your latest PDF (same name).
- **Project / certificate links:** search `index.html` for `TODO`. Set the `href`, then delete the `hidden` attribute from that link.
- **Social image:** replace `assets/images/og-image.png` with a 1200×630 image. After deploying, change the `og:image` and `canonical` values to full `https://` URLs.
- **Accent colour:** edit `--accent` in the `:root` and `[data-theme="dark"]` blocks in `css/style.css`.

## Deploy on GitHub Pages
1. Create a new public repository on GitHub. Naming it `username.github.io` gives you the URL `https://username.github.io/`. Any other name gives `https://username.github.io/repo-name/`.
2. Upload the files so `index.html` sits at the repo root (drag and drop on GitHub, or `git init`, `git add .`, `git commit -m "Add portfolio"`, `git remote add origin <repo-url>`, `git push -u origin main`).
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then branch `main` and folder `/ (root)`, and save.
5. Wait one to two minutes, then open the URL shown on that page.

## Pre-launch checklist
- [ ] Resume PDF is current and downloads
- [ ] Photo displays correctly
- [ ] Email, phone, LinkedIn and GitHub links work
- [ ] `canonical` and `og:image` use your live URL
- [ ] Project and credential links added where available (or left hidden)
- [ ] Tested on a phone, in dark mode, and with keyboard only
- [ ] Run Lighthouse in Chrome DevTools
