# IASI Documentation Template

Official template for documentation repositories in the IASI ecosystem.

It provides two independent publications:

- `01-user-guide`: user guide in HTML and PDF.
- `02-technical-guide`: technical guide in HTML and PDF.

Each manual is also an independent RStudio project. Both include the institutional pages under `common` and the visual identity under `resources`, including the corporate `ants.png` banner. The generated `publish/` directory is deployed to GitHub Pages.

## Create a documentation repository

1. Create the repository from this template.
2. Replace `IASI Documentation Template` with the public project name.
3. Replace `iasi-docs-template` with its repository name.
4. Replace pending pages with real documentation.
5. Enable GitHub Pages using **GitHub Actions** as its source.

## Build

```text
iasi-dev build repository-name-docs
iasi-dev publish repository-name-docs
iasi-dev deploy --full -m "publish documentation" repository-name-docs
```

The template has no external service or extension requirements.
