# Polymarket dashboard

A single self-contained page (`index.html`). All chart data is embedded in the
file; Plotly is loaded from a CDN, so the only requirement to view it is a
browser with internet access. There is no build step.

## Host on GitHub Pages

Option A, this folder as its own repo:

1. Create a new GitHub repository.
2. Push the contents of this folder so that `index.html` sits at the repo root.
3. In the repo, go to Settings, then Pages. Set Source to "Deploy from a
   branch", branch `main`, folder `/ (root)`.
4. The dashboard goes live at `https://<user>.github.io/<repo>/` within a minute.

Option B, inside a larger repo:

Move this folder to `docs/` and set the Pages source to the `/docs` folder, or
publish it on a `gh-pages` branch.

## Updating

Re-run the notebook, copy the new `index.html` produced by the dashboard cell
into this folder, and push.
