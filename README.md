# xiaozhou-li.github.io

Personal academic website for Xiaozhou Li, built as a static site and deployed with GitHub Pages. The repository contains multiple standalone HTML pages along with shared assets under `css`, `js`, `img`, and `files`.

## Project layout

- `home.html`, `onepage.html`, `background.html`, etc. — entry pages for different sections of the site.
- `css/` — compiled stylesheets served to the browser.
- `scss/` — Sass sources; update these first, then compile to `css/`.
- `js/` — JavaScript helpers and vendor scripts.
- `img/`, `files/` — static media and downloadable assets.
- `mail.php` — simple form handler for the contact page.

## Local development

1. Serve the repository root with any static server to preview locally, e.g.:
   ```bash
   python3 -m http.server 8000
   ```
2. Edit the relevant HTML or asset files, then refresh the browser.

### Working with styles

If you update Sass files, rebuild the CSS before committing:
```bash
sass --no-source-map scss:css
```
Feel free to use `sass --watch scss:css` during development for automatic recompilation.

## Deployment

Push changes to the `main` branch (or the branch configured in the repository settings) and GitHub Pages will publish the updated site automatically. Always verify the site locally before pushing.

## Contributing

This repository is maintained personally; please open an issue before proposing larger changes. When sending patches, keep HTML/CSS style consistent with the existing files and include any necessary assets.
