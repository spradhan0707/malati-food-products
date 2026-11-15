# Malati Food Products Catalogue (updated)

## Files
- `index.html` — public catalogue with English, Odia and Hindi language selector.
- `admin.html` — English-only admin panel for adding/editing/deleting products and uploading product images.
- `products.json` — updated from `PINELAB.xlsx` using the SP (Selling Price) column.
- `logo.png` — Malati logo.
- `product-images/` — place for product images uploaded through the admin panel.

## Product categories
The public catalogue uses these exact filters: All Products, Millets/Rice, Other, Atta, Sattu, Spices. Workbook category `Others` is mapped to `Other`.

## Publish on GitHub + Netlify
Upload/replace the package files in the root of your existing GitHub repository. Keep Netlify publish directory as `.` and build command blank. Netlify will redeploy after the commit.

## Admin
Open `/admin.html`. Enter GitHub owner, repository, branch and a fine-grained GitHub token scoped to this repository with Contents read/write permission. The token is held in the browser tab and is not part of the website source. Keep it private and revoke it if exposed. Admin UI is English; optional Odia/Hindi product and category fields can be filled for multilingual display.

## Language notes
The public page translates interface labels and category names. Product names display Odia/Hindi values when those optional translations are populated; otherwise they fall back to the English product name. Prices and numerals remain in English numerals.
