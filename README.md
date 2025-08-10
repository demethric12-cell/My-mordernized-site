# Dekpoy Enterprise — Jekyll + Netlify CMS (modernized)

This is a ready-to-deploy Jekyll site with Netlify CMS integration.

## What is included
- Jekyll site with responsive modern design
- Products stored as Markdown in `_products/`
- Netlify CMS admin in `/admin` to manage products (requires Netlify Identity + Git Gateway)

## How to use
1. Replace placeholder images in `assets/images/` or upload via CMS (uploads go to `/uploads`).
2. Update `_config.yml` `url` to your deployed site's URL.
3. Commit and push to your GitHub repo.

## Deploying
- **Vercel**
  - Import repository into Vercel.
  - Set build command: `bundle exec jekyll build`
  - Set output directory: `_site`
- **Netlify (for Identity)**
  - Create a free site on Netlify using this repo (one-time).
  - In Netlify site dashboard, enable **Identity** and then **Git Gateway**.
  - Invite your email under Identity -> Invite users.
  - Keep `admin/config.yml` backend as `git-gateway`.
  - Open `https://<your-site>/admin` and log in via Netlify Identity to manage products.

## Notes
- If you prefer to use GitHub OAuth directly, replace backend with `github` and add `repo: yourusername/your-repo`.
- Videos can be YouTube links (the template auto-embeds) or direct video URLs stored in `uploads/`.

