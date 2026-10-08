# NÖMÄD Inferno animated overlay

A transparent, 16:9 animated overlay using the exact supplied PNG. No dependencies or external scripts.

## Preview
Open `index.html` in a desktop browser. The center should show whatever is behind the browser window (transparent rendering depends on the app). To inspect effects against a dark background, add a temporary background in developer tools; do not publish an opaque background.

## Publish to GitHub Pages
1. Create a public repository, e.g. `nomad-inferno-overlay`.
2. Upload `index.html` and `nomad-frame.png` to the repository root.
3. Settings > Pages > Build and deployment: Deploy from a branch, `main`, `/ (root)`; Save.
4. Wait for deployment and open `https://YOUR-USERNAME.github.io/nomad-inferno-overlay/`.
5. In PRISM Mobile ScreenCast, add a Web source using the URL. Test that the center is transparent and the effects animate on your particular device.

## Custom domain (optional)
Use `overlay.rootaccess.gg` rather than changing your existing main site's DNS. In Pages > Custom domain enter `overlay.rootaccess.gg`, then create a DNS CNAME record with host `overlay` pointing to `YOUR-USERNAME.github.io` (no https or repository path). Enable HTTPS after DNS verification. Do not alter the root domain records if it already hosts a site.

## Tuning
Add `?speed=0.75` for slower effects or `?speed=1.5` for faster ones. Mobile performance may vary. The original frame remains unchanged.

## Notes
Some PRISM Web sources may not preserve transparency or may behave differently on ScreenCast depending on platform/version. Test privately before using live. This is a first animation pass: glows and highlights, not actual fluid lava or independent animated skull artwork.
