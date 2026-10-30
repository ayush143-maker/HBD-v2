# HBD-v2

HBD-v2 is a personalized birthday microsite with a message, interactive gift, cake, five wish balloons, and four photo slots. The top-level `index.html` is the page entry point. The recipient and sender can be supplied in the URL, making it possible to personalize the greeting without editing the page’s copy for each visit.

## Preview locally

Open `index.html` in a browser, or serve the repository directory:

```sh
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000). No dependency installation or build scripts are listed. Cormorant Garamond and Manrope load from Google Fonts and require network access for those fonts.

## Personalize and interact

Add URL parameters such as `?name=Priya&from=Rahul` to set the recipient and sender. Values are trimmed to 24 characters; the recipient’s first character is capitalized. The provided values are inserted into the page text, and a supplied name also updates the document title. The displayed date comes from the browser’s locale and current date, not a fixed birthday date. Review the resulting text and URL before sharing.

Tap the gift card to toggle between its closed and voucher views. The cake takes two taps to light and then blow out its candle; there is no control to relight it afterward. Each of five balloons reveals an individual wish when popped. After all five are popped, a completion message and re-inflate control appear.

## Photos, motion, and files

The four photo slots reference `images/photo-01.jpg` through `images/photo-04.jpg`. Missing images are replaced by inline SVG illustrations, and some slots load lazily. Keep those relative paths valid when publishing or update the references in `index.html` if you move the photos.

Sections reveal as they enter the viewport. A reduced-motion CSS mode removes or shortens animations and transitions. The page holds personalization and interaction state in its scripts: it makes no application API calls and uses no local or session storage. Reloading resets gift, cake, and balloon interactions; personalization can be applied again through the URL. Edit the message, layout, font references, and behavior in `index.html`. For static publication, include that page and the referenced images, and preserve their relative paths.