# Netlify Ghost Forms Labeler

A Netlify-hosted signup endpoint for Ghost CMS. An embedded form on your Ghost site posts `firstName`, `lastName`, and `email` to a Netlify Function (`netlify/functions/create-member.js`), which creates the member through the Ghost Admin API with a `Netlify` label and redirects to a thank-you page (via `public/_redirects`).

Deploy on Netlify and set two environment variables:

- `GHOST_ADMIN_URL` — your Ghost site's URL
- `GHOST_ADMIN_API_KEY` — a Ghost Admin API key

The `index.html` in this repo is just a minimal "form is live" marker — the form itself lives on the Ghost site, so there's no site to screenshot here.

Companion to [mvvk-space/ghost-labeler](https://github.com/mvvk-space/ghost-labeler), which labels existing members.

**Live (marker page):** https://mvvk-space.github.io/netlify-ghost-forms-labeler/
