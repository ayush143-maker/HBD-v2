# HBD-v2

A minimal birthday microsite built around a personal message and a sequence of celebratory sections. The single-page experience is contained in the top-level `index.html`.

## Preview locally

Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No package manager or build command is required. Content and visual sequence are defined in `index.html`; after editing, review the message and preserve the section order. No deployment configuration is documented.

## Personalizing the page

The page title is “A birthday page ✦”. Update the visible message and title together when adapting the page, and keep the existing section order when changing the celebratory sequence. The document links to Cormorant Garamond and Manrope through Google Fonts; if you change the typefaces, update the font link and the corresponding styling in `index.html` together.

The root file list contains no separate media or asset directory. If you add an image or other asset, make sure its reference in `index.html` points to its actual location. Preview the finished page locally to review the message, typography, and section sequence.