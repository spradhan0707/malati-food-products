# Malati Food Products catalogue

## Files
- `index.html` — public product catalogue
- `products.json` — product data (98 initial products)
- `logo.png` — Malati logo
- `admin.html` — browser-based product manager

## Deploy
1. Upload all four files to the root of the GitHub repository.
2. Connect the repository to Netlify.
3. Leave build command blank and publish directory as `.`.
4. Public catalogue: `https://YOUR-SITE.netlify.app/`
5. Admin page: `https://YOUR-SITE.netlify.app/admin.html`

## Product management
1. Open `/admin.html`.
2. Create a GitHub fine-grained personal access token restricted to this repository.
3. Grant **Contents: Read and write** permission and set an expiry.
4. Enter GitHub owner, repository, branch (`main`) and token in the admin page.
5. Click **Connect & load products**.
6. Add/edit/delete products. You can also edit cells directly in the table.
7. Click **Save all changes to GitHub**. This commits `products.json`; Netlify automatically redeploys the site.

The token is held in browser session storage only. It is not embedded in the public website or saved in the repository. Do not share it. Anyone who obtains the token can change the repository contents within its granted permissions.

The admin URL is not a substitute for access control: the GitHub token is the actual write authorization. Use it only on a trusted device, sign out/clear the connection after use, and revoke the token in GitHub if it is exposed.

## Initial product data
Imported from the consolidated Malati Excel workbook; selling prices use the SP column. Confirm all prices before publishing.
