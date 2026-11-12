# Michael Kofler – CV

Source of my personal academic CV website. I am a PhD student at the
[Institute of Lightweight Design and Structural Biomechanics](https://www.tuwien.at/mwbw/ilsb/), TU Wien,
working on shape and topology optimization with neural-network-based geometry parametrizations.

🌐 **Live site:** <https://mkofler96.github.io/cv/>

[![Screenshot of the CV website](./.github/preview.jpg)](https://mkofler96.github.io/cv/)

## Featured project: KoFEM

[**KoFEM**](https://kofem.org/) is my open-source finite element solver that runs entirely in the browser.
Import a STEP file, mesh it, apply supports and loads, and solve locally, with no installation and no data leaving your machine.

- 🔗 Website: <https://kofem.org/>
- 💻 Code: <https://github.com/mkofler96/KoFEM>

## What's on the site

- **Biography, experience & education**: [`content/authors/admin/_index.md`](content/authors/admin/_index.md)
- **Projects**: [`content/project/`](content/project/)
- **Publications**: [`content/publication/`](content/publication/), generated from [`bib/bibliography.bib`](bib/bibliography.bib)
- **Conference presentations**: [`content/event/`](content/event/)
- **Posters**: [`content/poster/`](content/poster/)
- **Homepage layout** (section order): [`content/_index.md`](content/_index.md)

## Local development

The site is built with [Hugo](https://gohugo.io/) (extended, v0.136.5) and the
[Hugo Blox résumé theme](https://github.com/HugoBlox/theme-resume).

```bash
hugo server
```

Then open <http://localhost:1313/>.

### Updating publications

Add the BibTeX entry to `bib/bibliography.bib`, then run:

```bash
pip install academic
academic import bib/bibliography.bib content/publication/ --compact
```

### Adding a project

Create `content/project/<name>/index.md` (see [`content/project/kofem/index.md`](content/project/kofem/index.md))
and optionally put a square `featured.png` thumbnail next to it. For logos, use a transparent `featured.png` and set
`image.background: transparent` so the logo is shown whole and centered on the card's own color instead of cropped on narrow screens
(handled by the card override in [`layouts/partials/views/card.html`](layouts/partials/views/card.html)).

## Deployment

Every push to `main` builds the site and deploys it to GitHub Pages via
[`.github/workflows/publish.yaml`](.github/workflows/publish.yaml).

## Credits

Based on the [Hugo Blox résumé template](https://github.com/HugoBlox/theme-resume) by George Cushen (MIT License, see [`LICENSE.md`](LICENSE.md)).
Banner photo from [Unsplash](https://unsplash.com/).
