# Isabelle Borucki — Research & Projects

A responsive, buildless personal academic website prepared for `isaborucki/isabelleborucki`.

## Publish with GitHub Pages

1. Upload the contents of this folder to the repository's `main` branch, keeping `.github/workflows/pages.yml` and `.nojekyll` (hidden files).
2. In the repository, open **Settings → Pages → Build and deployment → Source**, and select **GitHub Actions**.
3. Open **Actions → Deploy research profile → Run workflow**, or push a change to `main`.
4. The workflow publishes the site at the URL reported in its deployment environment. The expected project URL is `https://isaborucki.github.io/isabelleborucki/`; this package alone does not enable hosting.

The workflow uses GitHub's built-in token. No personal access token, npm dependencies, or build step is needed. It deploys only the `public/` directory it assembles from the explicit website files.

## Edit the website

- `index.html`: profile, research narrative, teaching, navigation, and links.
- `content.json`: project cards, method tags, and publication metadata.
- `styles.css`: visual design and responsive layout.
- `app.js`: accessible project filters, publication search, year filter, and show-all control.
- `portrait.jpg`: portrait recovered from the owner's archived website. Credit: Bea Roth Photography. Photographer credit is retained on the site; no new license is asserted.

Profile text is currently in `index.html`. Some descriptive fields in `content.json` are retained as a portable content record; changing those fields does not replace the HTML biography.

Preview with `python3 -m http.server 4173` and visit `http://localhost:4173`. Use HTTP rather than opening `index.html` directly so the browser can fetch `content.json`.

## Hosting

GitHub Pages is configured to deploy this repository through GitHub Actions. The project URL is https://isaborucki.github.io/isabelleborucki/. 
