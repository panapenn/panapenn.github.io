# Personal academic website

Plain HTML/CSS/JS — no build step, works directly on GitHub Pages.

## Files
- `index.html` — all content. Search for `[` to find placeholders to replace.
- `style.css` — design (colors are the variables at the top; change `--accent` to recolor).
- `script.js` — dark-mode toggle and section highlighting.
- `assets/profile.svg` — placeholder photo. Add `assets/profile.jpg` and update the `<img src>` in `index.html`.
- `assets/cv.pdf` — add your CV here (linked from the sidebar).
- `.nojekyll` — tells GitHub Pages to serve files as-is.

## Publish on GitHub Pages
1. Create a public repo named `<your-github-username>.github.io`.
2. Push these files to the `main` branch:
   ```bash
   git init && git add . && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source: Deploy from a branch → main / root**.
4. After a minute the site is live at `https://<username>.github.io/`.

## Adding a publication
Copy one `<article class="pub">…</article>` block in the Publications section and edit it.
Put newer years above older ones.
