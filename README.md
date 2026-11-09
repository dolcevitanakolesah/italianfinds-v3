# Italian Finds — static website prototype

A responsive Russian-language classic-car showcase with an Italian editorial visual direction.

## Run locally
Open `index.html` in a browser, or run a local static server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy to Cloudflare Pages
1. Create a GitHub repository and push the contents of this folder to its root.
2. In Cloudflare, open **Workers & Pages → Create → Pages → Connect to Git**.
3. Select the repository.
4. Framework preset: **None**.
5. Build command: leave empty.
6. Build output directory: `/` (repository root).
7. Deploy.

No build step or server-side runtime is required.

## Replace the demo content
- Car listings and specifications: `app.js`, in the `cars` array.
- Main visual and editorial imagery: image URLs in `index.html`, `styles.css`, and `app.js`.
- Contact email: replace `ciao@italianfinds.example` in `index.html` and `app.js`.
- Brand colours and typography: CSS variables at the top of `styles.css`.

## Important
All cars, prices, mileage, specifications, and image assignments are illustrative placeholders. The remote photos are generic visual placeholders and may not depict the named model. Replace them with verified photographs and accurate vehicle details before publishing real offers.

The site uses hash-based client-side routes (`#/car/<id>`), so individual vehicle pages work on a static host without rewrite rules.
