# Stuff'd. — website

Static site for Stuff'd. upcycled stuffed pretzels. No build step.

## Run it
```
cd C:\Users\awvp3\stuffd-website
python -m http.server 5173
```
Open http://localhost:5173

## Pages
index (home) · shop · flavors (The Lineup) · upcycled · story · journal · stockists · wholesale · faq · contact

## Files
- `assets/css/style.css` — design tokens (colors, fonts) at the top, then every component
- `assets/js/site.js` — shared engine: header/menu/footer, page curtain, ScrollSmoother, cursor, magnetic buttons, text splits, marquees, bag drawer, product catalogue (`FLAVORS`, `PRODUCTS`)
- `assets/js/home.js`, `shop.js`, `flavors.js`, `upcycled.js` — page choreography

## Reusable data attributes
- `data-split="lines|chars|blur|scrub"` text reveals (SplitText)
- `data-scramble` scramble-in label · `class="idx"` mono index label · `data-reveal` fade-up batch · `data-count="41"` counter
- `data-bite="original" data-cut` draws a pretzel bite · `data-float` · `data-spin`
- `data-speed` / `data-lag` ScrollSmoother parallax · `data-magnetic` · `data-cursor="View"`
- `data-add="id"` add to bag · `data-salt` tap for a salt burst

Type: Geist (headlines + body), Geist Mono (labels), Fraunces (logo only). GSAP 3.13 (all plugins, free) loads from jsDelivr.
After editing CSS/JS, bump the `?v=` number on the asset links so browsers fetch the new files.
Copy, reviews, partner bakeries, stockists and impact numbers are placeholders — replace before launch.
