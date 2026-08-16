# WishBloom

A warm, playful birthday-wish experience by @Selfish_Senpaiii.

## This build
- Recipient experience now has a pinned ⚙️ settings control.
- Sounds can be toggled independently.
- Soft synthesized background music starts after the first user interaction (mobile autoplay rules), loops through gentle chord progressions, and has a volume slider.
- Music continues across the recipient experience and final reveal.
- Mini-games were rebuilt with more varied interactions: birthday clue, hidden cat grid, heart hunt, balloon popping, and mystery gift.
- Wrong answers always remain playful and never block progress.
- Correct answers advance automatically instead of leaving the user waiting on an extra intermediate card.
- Final reveal still includes confetti, balloons, cake/reveal flow, personalized writing, photos, wishes, the one-last-thing section, and the creator CTA.

## Running locally
Open `index.html` in a browser. For the most reliable shareable-link testing, serve this folder over HTTP (for example with GitHub Pages or any static web host).

## Static-link architecture
The current static build encodes the wish configuration into the shareable URL. This means a full shareable URL can carry the wish to another device once the site itself is hosted.

The short `WB-XXXX-XXXX` code is a display code only in this static build. True cross-device lookup from the short code alone requires a backend/database such as Supabase or Firebase.

## Audio note
The music is generated with Web Audio rather than a copyrighted song or external audio file. Browsers commonly block autoplay, so WishBloom starts the music after the first tap/click when Music is enabled.
