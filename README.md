# bitecode.ltd

The company site for Bitecode Ltd, served at [bitecode.ltd](https://bitecode.ltd).

It is plain HTML and CSS in `site/`, with no build step, scripts, cookies or tracking. Pushing to `main` deploys it to GitHub Pages through `.github/workflows/pages.yml`.

## Preview

```bash
python3 -m http.server 4173 --directory site
```

Then open http://localhost:4173.

## Check

```bash
bunx @biomejs/biome@2.5.12 ci .
```

## Files

- `site/index.html`: the home page: our products, services, process and contact
- `site/legal/index.html`: company, privacy and product terms links
- `site/404.html`: served by Pages for unknown paths
- `site/products/`: product icons
- `site/logo.svg`: the BiteCode wordmark and B mark as SVG symbols, used with `<use href="logo.svg#wordmark">`
- `site/fonts/`: Nunito, under the SIL Open Font License (`Nunito-OFL.txt`)
- `site/CNAME`: the custom domain

The paths in `logo.svg` and `favicon.svg` come from the BiteCode brand SVGs; replace them with new path data from the brand files rather than redrawing them.
