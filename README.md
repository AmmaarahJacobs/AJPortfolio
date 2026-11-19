# AJPortfolio

Portfolio site for Ammaarah Jacobs — software engineering and UX.

Single static page (`index.html`), no build step. Open it directly or serve the
folder.

## Structure

```
index.html              the whole site (markup, styles, project data)
img/                    CV, photos and other static assets
projects/               folders for projects that are not on GitHub
projects/README.md      how to add one
```

## Adding work

- **GitHub projects** — edit the `<div class="work-list">` block in `index.html`.
- **Everything else** (in-progress work, case studies, private or offline
  projects) — add a folder under `projects/` and an entry to `LOCAL_PROJECTS`
  at the bottom of `index.html`. See `projects/README.md`.

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```
