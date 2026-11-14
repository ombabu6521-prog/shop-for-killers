# SHOP. FOR. KILLERS

A static website, ready to publish with GitHub Pages.

## Publish the site

1. Sign in to [GitHub](https://github.com/) and create a **public** repository, for example `shop-for-killers`.
2. Install and open [GitHub Desktop](https://desktop.github.com/). Add this website folder as a local repository, then publish it to the public GitHub repository you created.
3. On GitHub, open the repository's **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
4. Open the **Actions** tab and wait for **Deploy website to GitHub Pages** to finish successfully. The workflow publishes the site on every push to `main` or `master`.
5. In **Settings → Pages**, set the custom domain to `shop.for.killers.in` and enable **Enforce HTTPS** when it becomes available. The `CNAME` file in this folder also declares that domain for deployments.
6. In the DNS settings for `killers.in`, add a **CNAME** record with host/name `shop.for` pointing to `YOUR-USERNAME.github.io` (replace this with the username from your GitHub Pages URL). DNS changes can take time to propagate. Then visit `https://shop.for.killers.in`.

If you have not configured the custom domain yet, the Pages URL shown in **Settings → Pages** remains available. For a repository named `shop-for-killers`, it will usually be `https://YOUR-USERNAME.github.io/shop-for-killers/`.

The site is static and needs no build step, backend, or package installation. Keep `.github/workflows/pages.yml` in the repository so GitHub can deploy updates.

## Website structure

- `index.html` is the home page and category overview.
- `red/index.html` lists RED topics. Each topic has its own page in `red/`; the mechanics topic includes three nested topic pages.
- `purple/index.html` is the PURPLE category landing page.
- `styles.css` contains shared responsive styles for all pages.

Add future RED topic content to its matching page in `red/`. Add future category materials to that category's page, then commit and publish the update; GitHub Actions will deploy it automatically.
