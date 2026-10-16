# GY NEXUS LIMITED Website

This repository contains the official corporate website for GY NEXUS LIMITED. It is a standalone static website and is completely separate from the existing GY DATA application repository.

## Website purpose

The site presents GY NEXUS LIMITED as a Nigerian technology and digital solutions company, with GY DATA positioned as one of the company’s products.

## Repository structure

- `index.html` — home page
- `about.html` — about page
- `services.html` — services overview
- `products.html` — product overview
- `gy-data.html` — dedicated GY DATA page
- `contact.html` — contact page
- `privacy.html` — privacy policy
- `terms.html` — terms of service
- `404.html` — custom 404 page
- `site-config.js` — centralized editable company and product configuration
- `assets/css/style.css` — site styling
- `assets/js/main.js` — site behavior logic
- `assets/images/` — logos and favicon
- `robots.txt` — search engine guidance
- `sitemap.xml` — sitemap
- `.github/workflows/deploy-pages.yml` — GitHub Pages deployment

## Editing company information

Open `site-config.js` and update the `company` object:

- `name`
- `rc`
- `tagline`
- `email`
- `phones`
- `address`
- `baseUrl`

## Editing GY DATA information

Update the `gydata` object in `site-config.js`:

- `title`
- `description`
- `url`

The project repository included in the site remains only a reference link and is not modified or copied.

## Updating contact details

Edit the values in `site-config.js` under `company`. The phone links and email links use these values.

## Changing prices or plans later

If pricing is added later, keep it in `site-config.js` rather than scattering it across HTML files.

## Deploying with GitHub Pages

1. Push changes to the `main` branch.
2. In GitHub, go to Settings → Pages.
3. Set source to GitHub Actions.
4. The workflow in `.github/workflows/deploy-pages.yml` will publish the website automatically.

## Custom domain

To use a custom domain later, add your domain in a `CNAME` file and configure DNS for GitHub Pages. Also update `site-config.js` `company.baseUrl` to your live domain.

## Security

Do not commit API keys, passwords, tokens, or payment credentials. Keep any real integration secrets in a secure server environment or GitHub Actions secrets if needed.
