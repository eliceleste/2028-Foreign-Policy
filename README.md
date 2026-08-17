Map the 2028 Field — interactive map

This repository includes a single-page interactive map (foreign-policy-map.html) that lets anyone place public figures on two axes and share their board via a URL fragment. The app is fully client-side — no server required.

How to publish (GitHub Pages)

1. Fork or clone this repository.
2. Ensure the file foreign-policy-map.html is present at the repo root (or keep index.html which redirects to it).
3. Option A (manual): In your repository settings -> Pages, set the source to the main branch (or a branch you prefer) and the root (/). Save. Your site will be served at https://<your-username>.github.io/<repo-name>/
4. Option B (automatic, recommended): Keep the provided GitHub Actions workflow (in .github/workflows/deploy-pages.yml). On push to the main branch the action will publish the repository root to GitHub Pages automatically.

Sharing maps

- Place dots on the board, then click "Copy share link". The link encodes your board in the URL fragment (no server). Paste and share.

Customizing

- Edit ROSTER_REP and ROSTER_DEM arrays inside foreign-policy-map.html (JS block) to change the chips shown.
- Modify ELI_MAP to change the reference placements.

License

This project is permissively licensed for public use. Add a LICENSE file if you want a specific license.

If you'd like, the repo can be set up to auto-deploy on push to the default branch — the included workflow shows one approach.