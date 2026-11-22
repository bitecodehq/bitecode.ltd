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

- `site/index.html`: the home page and product list
- `site/legal/index.html`: company, privacy and product terms links
- `site/404.html`: served by Pages for unknown paths
- `site/products/`: product icons
- `site/fonts/`: Nunito, under the SIL Open Font License (`Nunito-OFL.txt`)
- `site/CNAME`: the custom domain

The logo paths in the pages come from the BiteCode brand SVGs; edit the SVG source and paste the new path data in rather than redrawing them.
