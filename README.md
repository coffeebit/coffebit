# Coffebit Website

This repository contains the source code for the Coffebit website.

## Deployment to GitHub Pages

This website is automatically deployed to GitHub Pages via `gh-pages`. To deploy manually, run:

```bash
npm install
npm run deploy
```

## Connecting your Custom Domain (Squarespace)

1. Go to your Squarespace Domain dashboard.
2. Select your domain (`coffebit.com`) and navigate to **DNS settings**.
3. Add the following **A Records** pointing to GitHub Pages IP addresses:
    * `185.199.108.153`
    * `185.199.109.153`
    * `185.199.110.153`
    * `185.199.111.153`
4. Add a **CNAME Record**:
    * Name: `www`
    * Data: `coffeebit.github.io`
5. On GitHub, go to your repository's **Settings** -> **Pages**.
6. Under "Custom domain", enter `coffebit.com` and click **Save**. This will automatically add a `CNAME` file to your root directory.
7. Tick **Enforce HTTPS** (this may take up to 24-48 hours to provision the SSL certificate).
