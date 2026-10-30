# HBD-v2

HBD-v2 is a birthday microsite built around a personal message and celebratory sections. Its top-level `index.html` is the page entry point, with the document title “A birthday page ✦”.

## Preview locally

Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). No dependency installation or build scripts are listed. The page requests Cormorant Garamond and Manrope from Google Fonts, so the fonts depend on network access.

## Editing and review

The page content and typeface references are in `index.html`. If changing the typefaces, update both the font link and its corresponding styling. Preserve existing relative asset references when editing or adding assets, and verify that each reference matches a file at its published location.

Before sharing, review the personal message and section order. Preview the page at narrow and wide viewport sizes, checking the content and layout for clipping or overflow. If the Google Fonts requests are unavailable, check that the page remains legible with its fallback typography.

## Repository map

- `index.html` — page entry point, message, sections, and font references.

No deployment configuration or environment template is identified in the supplied repository content. For a static publication, include the entry page and any files it references.