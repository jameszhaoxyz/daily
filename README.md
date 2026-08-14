# Daily Notes — single-file blog

Dark, LaTeX-capable blog. **You only ever edit `posts.md`.**

## Post a note

Open `posts.md`, add a new block at the top of the post list:

```
=== 2026-08-15 | Title of today's note

Body in markdown. Inline math like $e^{i\pi}+1=0$ and display math:

$$\int_0^1 x^2\,dx = \tfrac13$$
```

Format: `=== YYYY-MM-DD | Title`. Everything until the next `===` is the body.
The site sorts by date automatically and uses the first paragraph as the preview.

The `#` line at the top of the file is the site title, the `>` line is the tagline.

## Run locally

Browsers block `fetch` on `file://`, so use a tiny server:

```
python3 -m http.server
```

Then open http://localhost:8000

## Host on GitHub Pages

1. Create a repo and push these files (`index.html`, `posts.md`, `style.css`, `.nojekyll`).
2. Repo → Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. Your site is live at `https://<user>.github.io/<repo>/`.

Daily posting is then: edit `posts.md`, commit, push. Nothing else.

## Files

- `index.html` — the whole site (renders markdown + KaTeX in the browser)
- `posts.md` — your content, the only file you edit
- `style.css` — dark theme
- `.nojekyll` — tells GitHub Pages to serve files as-is
