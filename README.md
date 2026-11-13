# SHOP. FOR. KILLERS

A static website, ready to publish with GitHub Pages.

## Publish the site

1. Sign in to [GitHub](https://github.com/) and create a **public** repository, for example `shop-for-killers`.
2. Install and open [GitHub Desktop](https://desktop.github.com/). Add this website folder as a local repository, then publish it to the public GitHub repository you created.
3. On GitHub, open the repository's **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
4. Open the **Actions** tab and wait for **Deploy website to GitHub Pages** to finish successfully. The workflow publishes the site on every push to `main` or `master`.
5. Visit the Pages URL shown in **Settings → Pages**. For a repository named `shop-for-killers`, it will usually be `https://YOUR-USERNAME.github.io/shop-for-killers/`.

The site is static and needs no build step, backend, or package installation. Keep `.github/workflows/pages.yml` in the repository so GitHub can deploy updates.

## Add category PDFs later

Place the PDF files in the website folder and link them from the relevant category section in `index.html`. Commit and publish the update; GitHub Actions will deploy it automatically.
