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

SUBSCRIBE
it's a mailto form by default (set SUBSCRIBE_ENDPOINT at the top of index.html to point it at Formspree/Buttondown instead).
