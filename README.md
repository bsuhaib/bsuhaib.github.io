# Portfolio (GitHub Pages)

Live site: **https://bsuhaib.github.io/** once this repo matches [bsuhaib/bsuhaib.github.io](https://github.com/bsuhaib/bsuhaib.github.io).

## What to publish

- `index.html` (main site)
- `images/` if you use images from HTML
- `.nojekyll` (tells GitHub not to run Jekyll on this static site)

Optional: keep `build_resume.js` in the repo for your own use; it is not served as the homepage.

## First-time push from this folder

```bash
cd "/Users/apple/Desktop/Suhaib/Portfolio"
git init
git branch -M main
git remote add origin https://github.com/bsuhaib/bsuhaib.github.io.git
git add index.html .nojekyll README.md .gitignore images/
git status   # review; add/remove paths as you like
git commit -m "Replace site with medical AI portfolio"
git push -u origin main
```

If the remote already has commits you care about, either **force-replace** the site (overwrite history — only if you are sure):

```bash
git push -u origin main --force
```

…or **clone** `bsuhaib.github.io` elsewhere, copy `index.html` and `.nojekyll` into it, commit, and push (no force).

## GitHub settings

Repository → **Settings** → **Pages** → Build and deployment: **Deploy from a branch**, branch **main**, folder **/ (root)**.

## Custom domain (later)

Same **Pages** settings: add your domain and follow GitHub’s DNS instructions at your registrar.
