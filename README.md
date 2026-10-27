# vu-nguyen-dev

One-page freelance site. Static HTML, no build step: open `index.html` in a browser.

## Edit
- **Prices:** the `<!-- PRICING -->` section in `index.html`.
- **Contact form:** create a free form at formspree.io and paste its ID into `FORMSPREE_ID` at the bottom of `index.html`. Until then, the form opens the visitor's email app addressed to vunguyenk@gmail.com.
- **Extension stats** (users, ratings) were taken from the Chrome Web Store on 2026-10-26. Update them by hand now and then.
- **Light/dark:** the color tokens are at the top of the `<style>` block. Dark mode follows the visitor's system setting.

## Deploy (GitHub Pages)
```bash
git remote add origin git@github.com:uyvunk/vu-nguyen-dev.git
git push -u origin main
```
Then go to Settings → Pages → Deploy from branch `main`, `/ (root)`. For a custom domain, add a `CNAME` file containing the domain and point DNS at GitHub Pages.
