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

## Content provenance

- Personal website archive supplied by the owner: https://web.archive.org/web/20250315032643/https://isabelleborucki.de/
- Archived research, teaching, and vita pages linked from that snapshot.
- ORCID biography and works: https://orcid.org/0000-0003-2076-4975
- Public ORCID API v3.0: person and works endpoints, retrieved 31 October 2026.

The publication list contains 51 records after deduplicating by DOI (or title where no DOI is present). It is a saved snapshot, not an automatic ORCID synchronization. Entries without a DOI link to the ORCID record. Corrections and other work types remain as recorded by ORCID. Historical projects and appointments are labeled accordingly. No contact email or additional project claims were invented.

## Hosting

GitHub Pages is configured to deploy this repository through GitHub Actions. The project URL is https://isaborucki.github.io/isabelleborucki/. A separate private Sites copy is available at https://research-profile-hub-oct31.brinybluff.chatgpt.site/.
