# WishBloom 🌸

A tiny birthday surprise made to feel personal.

## V7 polished build

- 1:1 square photo crop with zoom and positioning controls.
- Soft looping background music with a pinned settings button.
- Music volume + music/sound on/off controls.
- Browser-friendly audio startup: music begins as soon as the visitor interacts, because mobile browsers can block audible autoplay before the first tap.
- English, Hindi and Hinglish flows are kept language-consistent across the mini challenges and wishes.
- Natural, short birthday writing with proper punctuation.
- Final “One Last Thing” stays inside the birthday experience instead of returning to the homepage.
- Clean creator credits for Shivaayu with both Instagram profiles linked.
- Photos are cropped to 1:1 and compressed before encoding.
- Share payloads use browser compression where available to reduce URL length while keeping the site backend-free.

## Deploy

Upload `index.html` to the root of a static host such as GitHub Pages. No build step is required.

## Important static-link limitation

WishBloom V7 remains backend-free. The complete wish is stored inside the share URL, so the URL can still become long when photos are included, although V7 compresses the payload and aggressively resizes/crops photos.

The displayed share card no longer prints the enormous raw URL. **Copy Link** and **Share** still use the complete URL.

The short `WB-XXXX-XXXX` code is a friendly identifier, not a server-side database lookup. The recipient should receive the complete share link.

For genuinely short links such as `/wish/K7X9P2` with server-side retrieval, a database/storage backend will be required in a future backend version.
