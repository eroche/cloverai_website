# Legacy Site Snapshot Notes

Capture date:

- 2026-03-27

Source site:

- `https://www.clover.ai/`

Purpose:

- preserve the legacy Clover website's public HTML and referenced assets as reference material for the new site build
- keep first-party page shells separate from third-party hosted assets so reuse decisions are explicit

Directory meaning:

- `first_party/`: same-origin files captured from `www.clover.ai` / `clover.ai`
- `third_party/`: externally hosted files referenced by the site, including Webflow-hosted CSS, JS, images, icons, and fonts
- `pages/`: saved first-party HTML pages for the public site
- `screenshots/`: reserved for optional visual captures; not populated in this pass
- `manifests/`: machine-readable capture outputs, including `asset_manifest.tsv` and the initial `wget` crawl log

Classification rule:

- same-origin `clover.ai` and `www.clover.ai` content is treated as first-party
- any other host is treated as third-party

Captured page set:

- `index.html`
- `programming-language.html`
- `about-us.html`
- `services.html`
- `contact.html`

Captured host summary:

- `www.clover.ai`: 5 files
- `cdn.prod.website-files.com`: 35 files
- `assets-global.website-files.com`: 2 files
- `d3e54v103j8qbb.cloudfront.net`: 2 files
- `uploads-ssl.webflow.com`: 4 files
- `webflow.com`: 1 file

Important caveat:

- this snapshot is intended as a reusable reference set, not as a production-ready mirror
- the legacy site is a Webflow deployment, so most images, icons, CSS, JS, and fonts are third-party hosted rather than served from the Clover domain itself
- some externally referenced assets may still be decorative, duplicated, or unnecessary for the rebuilt site
