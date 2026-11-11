# The Site Handyman (thesitehandyman.com)

One-page freelance site. Static HTML, no build step: open `index.html` in a browser.

## Edit
- **Prices:** the `<!-- PRICING -->` section in `index.html`.
- **Contact form:** create a free form at formspree.io and paste its ID into `FORMSPREE_ID` at the bottom of `index.html`. Until then, the form opens the visitor's email app addressed to vunguyenk@gmail.com.
- **Extension stats** (users, ratings) were taken from the Chrome Web Store on 2026-10-26. Update them by hand now and then.
- **Vietnamese:** English text lives in the HTML. The Vietnamese for each element sits in its `data-vi` attribute, so edit both when you change copy. Link `https://thesitehandyman.com/?lang=vi` to open the page in Vietnamese. The toggle remembers the visitor's choice, and first-time visitors with a Vietnamese browser get Vietnamese.
- **Light/dark:** the color tokens are at the top of the `<style>` block. Dark mode follows the visitor's system setting.

## Deploy (GitHub Pages)
```bash
git remote add origin git@github.com:uyvunk/vu-nguyen-dev.git
git push -u origin main
```
Then go to Settings → Pages → Deploy from branch `main`, `/ (root)`. The `CNAME` file sets the custom domain `thesitehandyman.com`. At your registrar, add A records for `@` pointing to 185.199.108.153, 185.199.109.153, 185.199.110.153 and 185.199.111.153, plus a CNAME record for `www` pointing to `uyvunk.github.io`. Then turn on "Enforce HTTPS" in Settings → Pages.
