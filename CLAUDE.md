# Tobi Talk & Read

Live site: https://tobi-talk-and-read.netlify.app (Netlify project `tobi-talk-and-read`, linked to this repo's `main`).

## Netlify credits: keep usage near zero

- Every production deploy (a build of `main`) costs 15 credits. Branch deploys and deploy previews cost 0.
- `netlify.toml` has an `ignore` rule: a push to `main` only builds when the commit message contains `[deploy]`. Every other push to `main` is skipped.
- Do all work on the `draft` branch. Its branch deploy is free: https://draft--tobi-talk-and-read.netlify.app
- Batch changes. Only ship to `main` when the owner asks, with ONE commit or merge whose message contains `[deploy]`.
- Never put `[deploy]` in a commit message unless shipping to production is intended.
- Do not add Netlify Functions, Edge Functions, or other server compute. Keep the site a static single `index.html`.
