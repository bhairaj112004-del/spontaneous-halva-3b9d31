# AGENTS.md

## Architecture

This is a static, single-page site with no framework and no build step:

- `index.html` — the entire site (markup, embedded `<style>`, embedded `<script>`).
- `netlify.toml` — sets `publish = "."` so Netlify serves the repo root as-is.

## Conventions

- Keep everything in `index.html` unless the page grows enough to justify splitting CSS/JS into separate files — this project intentionally avoids build tooling.
- Content is in Hindi (targeting a local Rajasthan audience); preserve the Hindi copy when editing unless asked to translate.

## Non-obvious decisions

- The admission form has no backend: submitting it opens a pre-filled WhatsApp chat (`wa.me` link) to the institute's number instead of posting to a server or database. There is no persistent storage for form submissions — if that's needed later, wire up Netlify Forms or a Netlify Database (see the `netlify-forms` / `netlify-database` skills).
