# Ayush Rameja's 2025 Portfolio

Live archived portfolio: https://2025.ayush.im

Current portfolio: https://ayush.im

## Cloudflare deployment

The Vite frontend is served by the `old-portfolio` Cloudflare Worker at
`2025.ayush.im`. `wrangler.jsonc` publishes the `dist/` assets with a single-page
application fallback.

```bash
pnpm install --frozen-lockfile
pnpm run preview:cloudflare
pnpm run deploy:cloudflare
```

The preview script builds the frontend and starts a local Workers development
server. GitHub production builds and branch preview deployments are configured
separately after this migration is merged. The Mail link uses `wave@ayush.im`.

© Ayush Rameja
