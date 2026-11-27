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

## Temporary media dependency

The current artist visuals and June's PDF load using absolute URLs from `https://brownlotuspress.netlify.app/assets/`. This is deliberate: the text-code migration is complete, but **the media files have not yet been duplicated into this new repository**. The sites have distinct code and deployments but are not yet fully independent for media hosting. Copy the licensed assets into `assets/` here before removing the public URLs. Never delete the originals before validating the copies.

## Editing

- `index.html` — platform sections, featured roster, 2027 roadmap
- `styles.css` — platform design
- `app.js` — artist profiles, music-video records and event archive data
- `journal/index.html` — Listening Archive homepage
- `journal/archive.html` + `journal/archive.js` — archive catalogue
- `journal/articles/zamrock.html` — first editorial article
- `journal/journal.css` — journal styles

No framework or build command required. Keep the original June press kit live and unchanged during the migration.
