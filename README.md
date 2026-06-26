# Portfolio Site — Bushra Nazeer

A single self-contained `index.html` (no build step, no dependencies) — a fast,
accessible portfolio that links to the project repositories.

## Publish on GitHub Pages (free)

1. **Create a public repo.** Either:
   - `portfolio` → site lives at `https://bushra-nazeer.github.io/portfolio`, or
   - `bushra-nazeer.github.io` → site lives at `https://bushra-nazeer.github.io` (cleaner URL).
2. **Add the file.** Put `index.html` in the repo root and push:
   ```bash
   git init -b main
   git add index.html README.md
   git commit -m "Add portfolio site"
   git remote add origin https://github.com/bushra-nazeer/portfolio.git
   git push -u origin main
   ```
3. **Turn on Pages.** Repo → **Settings → Pages** → *Source*: “Deploy from a branch”
   → branch `main`, folder `/ (root)` → **Save**. Live in ~1 minute.

## Before you publish — 3 edits

1. Replace every `bushra-nazeer` with your real GitHub handle (and the LinkedIn slug).
2. As each project repo goes public, flip its card `data-status` from `building`
   to `live` and confirm the links resolve.
3. (Optional) Add a custom domain (e.g. `bushranazeer.dev`) under Settings → Pages.

## Customize

- **Colors / type** live in the `:root` CSS variables at the top of `index.html`.
- **Projects** are the `<article class="card">` blocks — edit title, role tags,
  tech chips, blurb, and links.
- **Experience / skills / certs** are plain HTML sections, easy to edit by hand.

## Alternatives to GitHub Pages

- **Netlify / Vercel** — drag-and-drop or git-connected deploys, free tier,
  custom domains. Use if you later rebuild this as a React/Next.js site.
