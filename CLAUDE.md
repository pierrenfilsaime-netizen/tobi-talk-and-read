# Neek AI (formerly Tobi Talk & Read)

Live site: https://tobi-talk-and-read.netlify.app (Netlify project `tobi-talk-and-read`).

## Netlify credits: keep usage near zero

- Every production deploy costs 15 credits. Bandwidth and requests for this small static page are negligible.
- The Netlify production branch is `live`. Branch deploys are off, so pushes to `main` cost nothing and do not deploy.
- Do all work on `main`. Batch changes.
- Ship ONLY when the owner asks: fast-forward `live` to `main` and push `live`, once per batch (`git push origin main:live`).
- Never push to `live` to test something.
- Do not add Netlify Functions, Edge Functions, or other server compute. Keep the site a static single `index.html`.
