# LLMs in Science — recovered content

A content-first Quarto starter recovered from the Internet Archive, using the March 21, 2025 homepage as the navigation reference. This is a historical recovery, not an editorial update of the site's advice.

## Review locally

```sh
cd /Users/rwatkins_1/research_projects/llminscience
quarto preview
```

To build a static site, run `quarto render`. The output is in `_site/`. GitHub Actions renders and publishes this directory to GitHub Pages on every push to `main`. Pull requests run the build without deploying.

## Content organization

- `index.qmd`: original homepage.
- `overview.qmd`: Overview and its three subpages.
- `resources.qmd`: Resource Hub and its seven subpages; partial archived listings only.
- `for-researchers.qmd`: For Researchers and its seven subpages.
- `for-reviewers.qmd`: For Reviewers and its seven subpages.
- `about.qmd`: About and its two subpages.

Subpages are consolidated under their original main-menu section titles. Local links point to the corresponding sections. Embedded media are retained as links, and available site-hosted images/downloads are saved in `assets/`.

## Recovery evidence

- `RECOVERY_REPORT.md`: coverage, dates, and limitations.
- `archive/manifest.json`: page and asset inventory, source URLs, resolved capture URLs, and recovery status.
- `archive/html/`: original archived WordPress HTML, retained before conversion.
- `archive/content/`: individual page Markdown, before section consolidation.
- `archive/wayback-url-index.json`: Wayback's successful HTML URL index used to check for additional static descendants; its timestamps are not necessarily the captures used for recovery.

The archive serves each page's available capture nearest the requested date. Captures can be older or newer than March 21, 2025; consult the manifest/report before treating these pages as a single-date snapshot. Original prose and typos are preserved. WordPress chrome, scripts, and interactive forms are omitted from the Quarto pages. Their original HTML remains available for inspection.

Resource Hub database records, pagination, search behavior, and submission handling have not been rebuilt. Captured listings are a useful starting point for a separate recovery. External links have been retained but not checked for currency. A new contact form or contact details will need to be chosen before publication.

## GitHub Pages

- Repository: https://github.com/ryanrwatkins/llminscience
- Website: https://ryanrwatkins.github.io/llminscience/
- Workflow: `.github/workflows/publish.yml` (Quarto 1.10.18).

Edit the `.qmd` source pages and push to `main` to update the site. Only `_site/` is deployed; original archive evidence remains in the repository. GitHub Pages uses the GitHub Actions publishing source. The recovery report describes the historical recovery stage, before publication.
