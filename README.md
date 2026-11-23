# blog

Personal blog built with [Astro](https://astro.build), deployed on Cloudflare Workers (static assets).

- New post: add `src/content/posts/<slug>.md` (frontmatter: `title`, `description`, `date`, optional `cover`, `draft`). Images go in `src/assets/posts/<slug>/`.
- Local: `npm install && npm run dev`
- Cloudflare Workers (static assets): build `npm run build`, deploy `npx wrangler deploy` (config in `wrangler.jsonc`).
- After the first deploy, set `SITE_URL` in `astro.config.mjs` to the live URL.
