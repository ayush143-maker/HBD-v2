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

These are actions to perform during review, not verified results or measured performance.

- Open `index.html` in a browser, or visit `http://localhost:8000` after starting the local server above.
- Read the message and scroll through the celebratory sections to check that their existing order is preserved after content edits.
- Check local image, audio, and font references in `index.html` against files that exist at those paths. The root file list contains no separate asset directory.
- If media is added, review its dimensions and file size for its role; avoid oversized media and remove assets only after confirming they are unused.
- The page links to Cormorant Garamond and Manrope through Google Fonts. Confirm that the external font dependency is intentional and the linked families are used. Keep the font link and matching styles aligned when changing typefaces; review any external script references before adding or retaining them.
- Inspect the layout at a narrow phone-sized viewport and a wide desktop-sized viewport. Check the message, section sequence, and typography at both sizes.

## Accessibility review checklist

These are future review actions, not claims that the page has been checked.

- Use the keyboard to move through the page and operate any links or controls. Check that all interactive elements can be reached without pointer input.
- Check that keyboard focus is clearly visible and distinguishable from the page backgrounds.
- Review any links or controls for meaningful names, and check that the birthday message and section sequence make sense without visual styling alone.
- Check text contrast against the backgrounds throughout the message and celebratory sections.
- If images or media are added, check whether meaningful content needs a text alternative and whether decorative assets can be ignored by assistive technology.
- Check any animation or transition with reduced motion requested, and consider reducing nonessential motion.