# kerstinweb – Claude Code Notes

## Deployment

This site is deployed via GitHub Pages from the `gh-pages` branch.
The `_site/` output folder is **gitignored** and not on `main`.

**To deploy changes:**

```bash
quarto publish gh-pages --no-prompt
```

This renders the site locally and pushes the output to the `gh-pages` branch.
GitHub Pages then deploys from there (usually within ~1 minute).

If `quarto publish` fails with a missing `_site/` directory error, render first:

```bash
quarto render && quarto publish gh-pages --no-prompt --no-render
```

**Note:** After deployment, a browser hard refresh (Cmd+Shift+R) may be needed to bypass caching.

## Structure

- `index.qmd` – Landing page (hero, about, skills, references, contact)
- `seminare.qmd` – Seminars page
- `cv.qmd` – CV page
- `custom.scss` – All custom styles
- `images/` – Photos and logos
