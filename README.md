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

## Configuration and data handling

This is a static page with no environment template or backend configuration listed. Keep credentials and private values out of `index.html` and other tracked files; anything embedded in the page is delivered to visitors and cannot be secret. Review the message and any added assets for personal or sensitive content before sharing or publishing them. The linked Google Fonts are retrieved from an external service by visitors' browsers.

## Browser and layout review checklist

This is a checklist for future review, not a report of completed browser testing or verified results.

- Open `index.html` in current versions of browsers relevant to the page's intended audience. Also review it through the local server above to check loading in a served-page context.
- Read the message and scroll through the celebratory sections to check that their existing order is preserved after content edits.
- Inspect the browser console during page load and while moving through the page. Investigate errors that affect the message or presentation.
- Inspect the Network panel for failed requests. Check that local assets you add resolve at the paths referenced in `index.html`; the root file list contains no separate asset directory. Check the Google Fonts requests for Cormorant Garamond and Manrope, confirm they are intentional, and consider the fallback appearance if they cannot load.
- Inspect the layout at a narrow phone-sized viewport and a wide desktop-sized viewport. Check the message, section sequence, and typography for clipping, overflow, or difficult-to-read text.
- If media is added, review its dimensions and file size for its role. Before removing assets, confirm they are no longer referenced.

## Accessibility review checklist

These are future review actions, not claims that the page has been checked.

- Use the keyboard to move through the page and operate any links or controls. Check that all interactive elements can be reached without pointer input.
- Check that keyboard focus is clearly visible and distinguishable from the page backgrounds.
- Review any links or controls for meaningful names, and check that the birthday message and section sequence make sense without visual styling alone.
- Check text contrast against the backgrounds throughout the message and celebratory sections.
- If images or media are added, check whether meaningful content needs a text alternative and whether decorative assets can be ignored by assistive technology.
- Check any animation or transition with reduced motion requested, and consider reducing nonessential motion.