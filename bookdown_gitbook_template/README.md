# bookdown gitbook template

This repo is a reusable template for a documentation website built with **bookdown** (gitbook style).

## Build locally

In R / RStudio:

```r
install.packages(c("bookdown", "rmarkdown"))
bookdown::render_book("index.Rmd")
```

The generated static site will be in `docs/`.

## Publish on GitHub Pages (easy mode)

1. Build locally so `docs/` exists.
2. Commit and push to GitHub.
3. GitHub repo Settings -> Pages:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /docs

## Publish with GitHub Actions (automatic)

A workflow is included at `.github/workflows/publish-bookdown.yml`.
It renders the site on each push to `main` and deploys to `gh-pages`.
Then set GitHub Pages to serve from `gh-pages` branch.
