# Deploying to GitHub Pages

This repo is already a static site (`index.html`), so the easiest setup is GitHub Actions + Pages.

## One-time GitHub setup

1. Push this branch to GitHub.
2. In your repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. Commit/push the workflow in `.github/workflows/pages.yml` (included in this repo).

After that, every push to `main` deploys the site.

## First deploy

If your default branch is `main`, the included workflow will run automatically after push.

Your site URL will be:

- `https://<your-username>.github.io/<repo-name>/`

## Important note about project pages path

Because this is likely a **project pages** site (not `username.github.io` root site), links should be relative (like `./about.html`) instead of absolute (`/about.html`) so they work under `/<repo-name>/`.

## If your default branch is not `main`

Edit `.github/workflows/pages.yml` and change:

```yaml
on:
  push:
    branches: ["main"]
```

to your branch name.
