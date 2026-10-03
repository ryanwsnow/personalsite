# personalsite

Static personal portfolio built with [Astro](https://astro.build/) and published with GitHub Pages.

## Run locally

Node.js 22.12 or newer is required.

```bash
npm install
npm run dev
```

The dev server starts at http://localhost:4321/.

## Build

```bash
npm run build
```

The static site is written to `dist/`. Preview that build locally with:

```bash
npm run preview
```

## GitHub Pages

Pushes to `main` run [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml). The workflow installs dependencies, builds the site with the official Astro GitHub Action, and deploys the `dist/` output to GitHub Pages. You can also run it manually from the Actions tab.

The site is built for the root of its domain, so local pages are at `/`. A custom domain will use that same root. GitHub’s default project address, https://ryanwsnow.github.io/personalsite/, is a subpath and will not match this setup.

Before the first deployment, open the repository on GitHub and set **Settings → Pages → Build and deployment → Source** to **GitHub Actions**.

No custom domain is configured.
