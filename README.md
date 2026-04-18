# Blackhole Pages

Public support pages for the Blackhole macOS app.

## Live Site

- Home: `https://blackhole.quirkgoose.com/`
- Support: `https://blackhole.quirkgoose.com/support.html`
- Privacy: `https://blackhole.quirkgoose.com/privacy.html`

## Repository Contents

- `index.html`
- `support.html`
- `privacy.html`
- `site.css`
- `.nojekyll`
- `CNAME`

## GitHub Pages Settings

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/ (root)`
- Custom domain: `blackhole.quirkgoose.com`

## DNS

Create this DNS record:

- Type: `CNAME`
- Host: `blackhole`
- Target: `quirkgoose.github.io`

## Contact

- `support+blackhole@quirkgoose.com`

## Update Workflow

This repository is updated from the app repo's `docs/` folder.

```bash
rsync -av --delete /Users/hanjungoo/workspace/blackhole/docs/ /Users/hanjungoo/workspace/blackhole-site/
cd /Users/hanjungoo/workspace/blackhole-site
printf 'blackhole.quirkgoose.com\n' > CNAME
git add .
git commit -m "Update Pages site"
git push origin main
```
