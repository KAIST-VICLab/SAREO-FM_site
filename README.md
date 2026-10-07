# SAREO-FM project page

Source of the project page for **SAREO-FM: Decoupled Semantic Supervision for SAR-EO Foundation Models**
(Jeonghyeok Do, Munchurl Kim; KAIST; arXiv preprint, 2026).

- Live page: https://kaist-viclab.github.io/SAREO-FM_site/
- Code repository: https://github.com/KAIST-VICLab/SAREO-FM

The page is plain HTML, CSS and JavaScript with no build step and no dependencies other than Google Fonts.
GitHub Pages serves it from the repository root (`.nojekyll` turns off Jekyll processing).

## Preview locally

Serve the folder over HTTP rather than opening `index.html` from disk, so that every path resolves as it does on GitHub Pages:

```bash
cd SAREO-FM_site
python3 -m http.server 8000
# then open localhost:8000 in a browser
```

## Layout

```
index.html                the page (results first: headline figure, the BRIGHT gallery and the SAR transfer figures,
                          quantitative results, then a compact method overview)
static/css/family.css     styles shared with the other KAIST-VICLab family pages (the same file on every page)
static/js/family.js       scripts shared with those pages: navigation, abstract toggle, pending links, BibTeX copy,
                          image lightbox, tabs, table scroll cues
static/css/style.css      SAREO-FM brand colours (top of the file), the gallery, the comparison slider, figures and tables
static/js/main.js         BRIGHT gallery (tile strips in a carousel) and comparison slider
static/images/            figures (web sizes + *_full for the lightbox), og.jpg (social preview) and the logo files
static/tiles/             per-input image tiles of the BRIGHT comparison for the interactive gallery
static/paper/             the paper (PDF)
```

## Logo

`static/images/logo.webp` is the hero logo (the SAREO-FM mark next to the wordmark, "SAREO" in ink `#1C2737` and
"-FM" in pink `#D63370`). `icon.png` is the mark used in the navigation bar and the footer, and `favicon-32.png`,
`favicon-64.png` and `apple-touch-icon.png` are the browser and home-screen icons made from the same mark.

## Links

- Paper: `static/paper/SAREO-FM.pdf`
- arXiv: the identifier is not assigned yet. Every arXiv link (hero button, footer, BibTeX) holds the placeholder
  `XXXX.XXXXX` and is shown as pending ("soon") until the placeholder is replaced by the real identifier.
- Code: https://github.com/KAIST-VICLab/SAREO-FM
