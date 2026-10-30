# HBD-v2

A birthday microsite built around a personal message and celebratory sections. The page is in the top-level `index.html` (title: “A birthday page ✦”).

## Preview locally

Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>. The page requests Cormorant Garamond and Manrope from Google Fonts, so those fonts depend on network access.

## Deployment-readiness checklist

The repository has a top-level `index.html` and no listed build scripts. The following are recommendations to check before and after publishing; they do not indicate that a deployment has taken place.

### Before publishing

- [ ] Use the repository root as the output directory so the top-level `index.html` is included.
- [ ] Keep asset and page references relative where appropriate, and verify that each reference points to a file at its published location. Preserve existing relative references when editing or adding assets.
- [ ] No environment configuration template is identified in the supplied repository files. Do not add environment configuration unless the project gains a template or a documented need for it.
- [ ] If changing the typefaces, update both the font link and the corresponding styling in `index.html`.
- [ ] Review the message and section order, inspect the layout at narrow and wide viewport sizes, and check any added asset references.

### After publishing

- [ ] Open the published page and review it in a browser.
- [ ] Confirm the page loads from its published location and that relative references resolve correctly.
- [ ] Review the layout at narrow and wide viewport sizes, and check that the Google Fonts load when network access is available.

## Contributor handoff

Keep changes scoped to the page and content being updated. Before handing off, describe what changed and note anything that still needs review. The checklist above is guidance, not a report of completed checks.

**Handoff summary:** Describe the changes and note anything that still needs review.

## Final release review

- Open `index.html` from the published location and confirm the page loads as expected.
- Test with network access available and keep a sensible fallback for externally loaded resources.
- Review the published result once on a narrow screen and once on a wider screen; treat this as a release check, not an automated test report.
