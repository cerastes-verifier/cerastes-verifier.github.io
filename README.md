<picture>
  <source media="(prefers-color-scheme: dark)" srcset="src/assets/cerastes-lockup-on-dark.svg">
  <img alt="Cerastes" src="src/assets/cerastes-lockup-on-light.svg" height="72">
</picture>

Source for [cerastes-verifier.github.io](https://cerastes-verifier.github.io), the website for Cerastes, a deductive verifier for C and C++. Built with [Astro](https://astro.build).

## Development

Requires Node 22.12 or later.

```sh
npm install
npm run dev       # dev server at http://localhost:4321
npm run build     # static output in dist/
npm run preview   # serve dist/ locally
```

## Layout

| Path | Contents |
|---|---|
| `src/pages/index.astro` | The site's single page |
| `src/assets/` | Logo files imported by pages |
| `public/` | Files served as-is: favicons, app icons, web manifest, social preview |
| `BRAND.md` | Brand guide: colors, typography, logo usage |

## Deployment

Every push to `main` builds the site and deploys it to GitHub Pages through `.github/workflows/deploy.yml`. In the repo's **Settings → Pages**, set **Source** to **GitHub Actions**.
