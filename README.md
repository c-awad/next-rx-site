# next-rx.com

The Next-Rx marketing site: a holding page and the privacy policy.

Deployed to GitHub Pages by `.github/workflows/deploy-site.yml` on every push
to `main`. The privacy policy is also copied to `privacy/index.html` at deploy
time so it is served at `/privacy`, which is the URL declared in the Play Store
listing.

`CNAME` binds the custom domain. Removing it silently unbinds next-rx.com, so
the workflow fails the build if it is missing.

The app source lives in a separate private repository.
