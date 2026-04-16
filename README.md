# Dheeraj Karanam — Portfolio

Personal portfolio website. Plain HTML + CSS, no build step, served statically via GitHub Pages.

## Stack

- HTML5, CSS3 (no JS framework)
- Fonts: Fraunces + Figtree + JetBrains Mono via Google Fonts
- Hosting: GitHub Pages

## Local preview

Just open `index.html` in a browser, or run a simple static server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying to GitHub Pages (user site)

This deploys to `https://dheeraj31104.github.io` (no subpath).

1. Create a new public repository on GitHub named exactly **`Dheeraj31104.github.io`** (the username must match yours).
2. From this folder, initialize git and push:

   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Dheeraj31104/Dheeraj31104.github.io.git
   git push -u origin main
   ```

3. In the GitHub repo, go to **Settings → Pages**. Under "Build and deployment", set:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / `(root)`
   - Save.

4. Wait ~1–2 minutes. Your site goes live at `https://dheeraj31104.github.io`.

## Updating content

Edit `index.html`, commit, push. Pages rebuilds automatically.

```bash
git add .
git commit -m "Update projects section"
git push
```

## File layout

```
.
├── index.html       # all page content
├── style.css        # full stylesheet
├── resume.pdf       # downloadable résumé (2-page)
├── .nojekyll        # tells Pages to skip Jekyll processing
├── .gitignore
└── README.md
```
