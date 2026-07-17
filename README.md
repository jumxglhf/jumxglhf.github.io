# jumxglhf.github.io

Personal academic homepage of Mingxuan (Clark) Ju — [jumxglhf.github.io](https://jumxglhf.github.io).

Built with [Jekyll](https://jekyllrb.com/) using the [al-folio](https://github.com/alshedivat/al-folio) theme.

## Editing content

- **About / bio:** `_pages/about.md`
- **News:** one file per announcement in `_news/`
- **Publications:** `_bibliography/papers.bib` (BibTeX; `selected={true}` entries appear on the homepage)
- **CV:** `_data/cv.yml` (rendered at `/cv/`) and the PDF at `assets/pdf/clark_mingxuan_ju_resume.pdf`
- **Life:** `_pages/life.md` with photos under `assets/img/life/`

## Local development

With Docker installed:

```bash
docker compose up
```

Then open <http://localhost:8080>. Alternatively, with Ruby ≥ 3.3:

```bash
bundle install
bundle exec jekyll serve
```

## Deployment

Pushing to `master` triggers `.github/workflows/deploy.yml`, which builds the site and
publishes it to the `gh-pages` branch. GitHub Pages must be configured to serve from
`gh-pages` (Settings → Pages → Deploy from a branch → `gh-pages` / root).
