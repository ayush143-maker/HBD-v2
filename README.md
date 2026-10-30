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

## Troubleshooting

Use these as diagnostic steps, not as claims that the page currently has a problem:

1. **Confirm the entry page.** Open the top-level `index.html`, or serve the repository directory and visit its root URL. Confirm the served directory if the expected message or sections are not shown.
2. **Check paths and local files.** Preserve relative paths for any assets added to the page. If one fails to load, confirm the file is present and its reference in `index.html` matches its location; no separate asset directory is listed at the root.
3. **Inspect browser diagnostics.** Check the console during page load and while moving through the page. In the Network panel, inspect failed requests and their URLs to help identify missing local files or other loading errors.
4. **Distinguish external fonts.** Cormorant Garamond and Manrope are requested from Google Fonts, so their loading depends on network access to that service. Check those requests separately from local assets and consider how the page looks if the fonts are unavailable.

## Configuration and data handling

This is a static page with no environment template or backend configuration listed. Keep credentials and private values out of `index.html` and other tracked files; anything embedded in the page is delivered to visitors and cannot be secret. Review the message and any added assets for personal or sensitive content before sharing or publishing them. The linked Google Fonts are retrieved from an external service by visitors' browsers.

## Browser and layout review checklist

This is a checklist for future review, not a report of completed browser testing or verified results.

- Review the page in current versions of browsers relevant to its intended audience.
- Read the message and scroll through the celebratory sections to check that their existing order is preserved after content edits.
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