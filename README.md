# Sessions on the Moon — Brown Lotus Records

This is the **independent Sessions on the Moon website** repository.

- **June on the Moon press kit** remains in [briisflash/juneonthemoon-presskit](https://github.com/briisflash/juneonthemoon-presskit).
- **Sessions on the Moon platform** is in this repository, on `main`.
- The journal is in `journal/`, with a researched introductory article under `journal/articles/`.
- `app.js` contains artist, video and past-session records.

## Netlify migration

Do not disconnect the existing live website until this new repository has been deployed and verified.

To connect a **new** Netlify preview, import `briisflash/brown-lotus-sessionsotm` from GitHub:
- branch: `main`
- base directory: blank
- build command: blank
- publish directory: `.`

Then verify `/`, `/#films`, `/#past-sessions`, `/#roadmap`, `/journal/`, `/journal/archive.html`, and `/journal/articles/zamrock.html`.

To retain the existing website address after verification, switch the existing Sessions on the Moon Netlify project to this repository using the Netlify project repository settings (if supported), or attach the desired domain to the new site.

## Media now hosted independently

The three files used by the platform are now stored in this repository under `assets/`:
- `june-hero-2.jpg`
- `june-photo-4.jpg`
- `june-presskit.pdf`

The Sessions platform points to those local media files. June's original press kit and media remain in the separate original repository. A clearly labeled external link to the **original June on the Moon press-kit site** is intentional and does not affect independent asset hosting.

The one-time asset import was completed by GitHub Actions (see `.github/workflows/import-press-assets.yml`).
The source project and the new platform are separate. Keep both websites active while testing the Netlify domain configuration.

## Editing

- `index.html` — platform sections, featured roster, 2027 roadmap
- `styles.css` — platform design
- `app.js` — artist profiles, music-video records and event archive data
- `journal/index.html` — Listening Archive homepage
- `journal/archive.html` + `journal/archive.js` — archive catalogue
- `journal/articles/zamrock.html` — first editorial article
- `journal/journal.css` — journal styles

No framework or build command required. Keep the original June press kit live and unchanged during the migration.
