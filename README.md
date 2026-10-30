# HBD-v2

A minimal birthday microsite built around a personal message and a sequence of celebratory sections. The single-page experience is contained in the top-level `index.html`.

## Preview locally

Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit http://localhost:8000. No package manager or build command is required. No deployment configuration is documented.

## Personalizing the page

The page title is “A birthday page ✦”. Update the visible message and title together when adapting the page, and keep the existing section order when changing the celebratory sequence. The document links to Cormorant Garamond and Manrope through Google Fonts; if you change the typefaces, update the font link and the corresponding styling in `index.html` together.

The root file list contains no separate media or asset directory. If you add an image or other asset, make sure its reference in `index.html` points to its actual location.

## Manual review checklist

These are actions to perform during review, not verified results.

- Open the known entry page, `index.html`, in a browser, or visit `http://localhost:8000` after starting the local server above.
- Read the message and scroll through the celebratory sections to check that their existing order is preserved after content edits.
- Check any image or media references in `index.html` against the assets' actual paths, especially if you added or moved assets.
- Inspect the layout at a narrow phone-sized viewport and a wide desktop-sized viewport. Check the message, section sequence, and typography at both sizes.
- If you changed typefaces, check that the Google Fonts link and the matching styles in `index.html` agree.
