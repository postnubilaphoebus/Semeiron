# ME/CFS & Long COVID biomarker atlas — results website

This is the **results website only**: the approved atlas layout, summaries, topic map and cited source text. There is no scraper, Python pipeline, API key, database or server application in this folder.

## Publish with GitHub Pages

1. Create a repository, then upload the **contents of this folder** into its root. `index.html`, `about.html`, `assets/` and `downloads/` must sit directly at the repository root. Preserve the folders and include `.nojekyll` (enable hidden files in your file manager if necessary).
2. In **Settings → Pages**, choose **Deploy from a branch**, select **main** and **/(root)**, then **Save**.
3. Once GitHub finishes deployment, use the **Visit site** link in Pages settings. Share that website URL, rather than the repository’s `index.html` source view.

No build command, GitHub Actions customization, API secret or backend is needed. All links use relative paths so project sites work under `https://USERNAME.github.io/REPOSITORY/` as well as at a domain root.

Official instructions: [configure GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site), [upload files](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).

GitHub's browser uploader accepts files up to 25 MiB each. This package splits the atlas into files smaller than 8 MiB; every file fits that limit. Upload the actual files and folders, not this folder's ZIP archive. A ZIP stored in the repository is not an unpacked website.

## Open locally

Open `index.html` in a recent browser with JavaScript enabled, keeping its assets alongside it. The data is loaded as local scripts, so no Python or development server is required. The original standalone `atlas.html` in the research run also remains unchanged.

The site initially loads approximately 36 MB of compressed/base64 atlas data. Loading progress is shown while the chunks arrive. Subsequent searches and evidence browsing run in the visitor's browser. The external paper and reference links open their respective source websites when selected.

## Files

- `index.html`: interactive atlas entry page.
- `about.html`: scope, methods, limitations and all 50 group descriptions.
- `assets/atlas.css`: layout and styling.
- `assets/atlas.js`: search, navigation, source-evidence display and data loading.
- `assets/atlas-data-*.js`: all text/data needed by the original viewer, split for upload.
- `downloads/taxonomy.json`: the complete curated topic map and assignment reasons.
- `snapshot.json`: dataset counts, export provenance and file hashes.
- `.nojekyll`: serve the static files directly.

This is a frozen inventory snapshot from 19 November 2026. Detailed high/low/normal extraction has not run. See `about.html` for how to interpret the evidence. No papers are removed or reclassified during website packaging. The original analysis files are kept separately.
