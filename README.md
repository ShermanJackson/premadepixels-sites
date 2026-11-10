# PremadePixels sample artist sites

Static files for GitHub Pages, intended to be served at **sites.premadepixels.com**.

This folder is the repository root. It contains a small index and two fictional artist sample sites, each built from a PremadePixels cover.

## Upload to GitHub Pages

1. Create a new GitHub repository and push this folder as the **root** of the `main` branch (not a subfolder). The included `CNAME` and `.nojekyll` files should sit at the repo root, alongside `index.html`.
2. In the repo, open **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**, branch to **main**, and folder to **/ (root)**. Save.
4. Under **Custom domain**, enter `sites.premadepixels.com` and save. GitHub should pick up the `CNAME` file in the repo.
5. At your DNS provider, add a **CNAME** record: host `sites` → `<username>.github.io` (use the GitHub Pages hostname for this account, for example `your-user.github.io`).
6. Wait for DNS to propagate, then tick **Enforce HTTPS** in the Pages settings.

The two sample sites (`/edrik-vohl/` and `/ione-merroway/`) include `<meta name="robots" content="noindex">` because the artists are fictional. The root index does not.

Do not re-export or recompress the cover images in `edrik-vohl/img/` or `ione-merroway/img/`. They are the original 780px files.
