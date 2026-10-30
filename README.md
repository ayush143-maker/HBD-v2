# HBD-v2

A birthday microsite built around a personal message and celebratory sections. The page is in the top-level `index.html` (title: “A birthday page ✦”).

## Preview

Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>. The page requests Cormorant Garamond and Manrope from Google Fonts, so those fonts depend on network access.

## Contributor handoff

Keep changes scoped to the page and content being updated. Preserve `index.html` and any existing relative references when editing or adding assets; check that references still point to the correct files. If changing the typefaces, update both the font link and the corresponding styling in `index.html`.

Before handing off or publishing, describe what changed and manually review the result. For example, check the message and section order, inspect the layout at narrow and wide viewport sizes, and confirm any added asset references are correct. This is a review checklist, not a report of completed checks.

**Handoff summary:** Describe the changes and note anything that still needs review.