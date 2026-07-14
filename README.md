# layers-of-vision

This repository is used for the content management, and hosting of, the Layers of Vision project website, led by Katharina Huseman at KCL Business School.
It supports an exhibition planned for the 18th of November 2022, acting as a supplement and enhancement for exhibition visitors with impaired vision.

Deployed at https://layersofvision.org

## About the exhibition

Layers of Vision is an art exhibition that explores the experiences and perspectives of blind and partially sighted (BPS) artists living in a world made for sighted people.

## For editors

Docs on how to add and update content is available in the [Wiki](https://github.com/kingsdigitallab/layers-of-vision/wiki/Wiki-for-Editors).

## Publishing

The site is built with Eleventy (11ty) from the `frontend/` folder and published
automatically — there is no manual deploy step.

1. Add or edit markdown/media in `frontend/` (e.g. `frontend/people/NN-name.md` for a new
   artist, or `frontend/<section>/index.md` for a page). Put images/audio in
   `frontend/assets/`.
2. (Optional) Preview locally: from the repo root run `npm ci`, then
   `cd frontend && npm run serve` and open http://localhost:8080.
3. Commit and push to the `main` branch.

That's it. Pushing to `main` triggers the **Build Eleventy** GitHub Action
(`.github/workflows/build.yml`), which builds the site and publishes it to the `gh-pages`
branch. GitHub Pages then serves it at https://layersofvision.org (usually within a minute
or two — watch the run in the repo's **Actions** tab).

> Do not edit the `gh-pages` branch directly — it is generated on every build and any manual
> changes will be overwritten.

## Release notes

### 1.1

- Added GoatCounter Analytics

### 1.0

- Accessibility improvements: added more sr-only spans to facilitate screen readear users' experience
- Added individual artist pages content
- Active links on artits index page
- Restored floorplan mao on the exhibition page
- Image size optimisation

### 0.2

- Removed floorplan from exhibition page

### 0.1

- Initial release
