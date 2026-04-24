# Enverse Domains

This repository currently contains a single static site in `enverse.com/`.

## Cloudflare Pages

- Project: `enverse-com`
- Production Pages URL: `https://enverse-com.pages.dev`
- Active custom domain: `https://www.enverse.com`
- Apex domain `enverse.com` is intentionally not attached to Pages.

## Publish Again

1. Change into the site directory:

   ```bash
   cd enverse.com
   ```

2. Log in to Wrangler if needed:

   ```bash
   npx -y wrangler login
   ```

3. Deploy the current static files to Cloudflare Pages:

   ```bash
   npx -y wrangler pages deploy . --project-name enverse-com --branch main
   ```

4. Verify the deployment:

   ```bash
   curl -I https://www.enverse.com
   ```

There is no build step. The deploy publishes the files in `enverse.com/` directly.
