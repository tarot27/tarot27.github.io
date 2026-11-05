# TAROT 2027 — editable Jekyll website

A multi-page Jekyll version of the TAROT 2027 site, using the same visual styling as the earlier standalone starter. This is **not** a fork or reproduction of the TAROT 2026 repository.

## Edit text — without HTML

Each section has its own Markdown file in the **repository root**:

| File | Page |
| --- | --- |
| `index.md` | Home |
| `about.md` | About |
| `programme.md` | Programme |
| `lecturers.md` | Lecturers |
| `organisers.md` | Organisers |
| `venue.md` | Venue |
| `accommodation.md` | Accommodation |
| `social-events.md` | Social events |
| `sponsors.md` | Sponsors |
| `past-editions.md` | Past editions |

To edit in GitHub: select the file → pencil icon → edit text **below the second `---`** → **Commit changes**. Do not delete the YAML front matter at the top. For navigation or layout changes edit `_layouts/default.html`, and for colours/layout edit `assets/style.css`.

## Publish to the `tarot27` organisation

1. Extract this ZIP to a normal folder. **Do not upload the ZIP itself.**
2. Open the GitHub repository `tarot27/tarot27.github.io` and upload **all files and folders inside** the extracted folder. `index.md` and `_config.yml` must be at the root; keep the `_layouts` and `assets` folders.
3. If the old standalone starter has already been uploaded, **remove the old `index.html`** before publishing. It would conflict with the new `index.md` homepage. The old root-level `style.css` and `script.js` are no longer used and can also be deleted.
4. Go to **Settings → Pages → Build and deployment → Source: Deploy from a branch**, select `main` and `/(root)`; save. GitHub Pages builds Jekyll automatically for branch deployments.
5. Check the **Actions** tab for build status, then open `https://tarot27.github.io/`.

This website will be **publicly accessible** once GitHub Pages is enabled. For private development, keep the repository private and do not enable Pages, or preview the site locally using Jekyll.

## Local preview (important)

**Double-clicking `index.md` will not preview this website.** Jekyll must first render the Markdown and templates.

If Ruby/Jekyll is available on your computer, open a terminal in the extracted folder and run:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000/` in your browser. Alternatively, publish it on GitHub Pages to see the rendered site.

## Known facts already included

- **7–10 June 2027**, Aalto University, Computer Science Building (Tietotekniikkatalo), Konemiehentie 2, Espoo, Finland.
- **7 June:** full day.
- **8 June:** half-day Summer School + half-day Secure Demo Day with universities; time order unspecified.
- **9 June:** half-day Summer School + tours + dinner.
- **10 June:** full day.

Unconfirmed speakers, exact times, hotels, sponsors, and registration details have **not** been invented.
