# Link Tree

A minimal, single-page link tree built with plain HTML and CSS. It puts your profile and all your important links in one place, with a soft glass-card design, subtle motion, and automatic light/dark themes.

## Features

- Clean, professional layout with a serif/sans type pairing (Fraunces + Inter)
- Frosted-glass link cards with smooth hover and entrance animations
- Automatic dark mode via `prefers-color-scheme`
- Responsive down to phone widths
- Respects `prefers-reduced-motion`
- No JavaScript, no build step

## Getting started

Open `index.html` in a browser. Or serve the folder locally:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Customizing

- **Profile:** edit the name, initials, tagline and status badge in `index.html`.
- **Links:** replace each `href="#"` and the placeholder email. To add a link, copy an `<a class="link">` block and give it the next `--i` value so the entrance animation stays staggered.
- **Colors:** change the CSS variables at the top of `style.css` (`:root` for light, the `@media (prefers-color-scheme: dark)` block for dark).

## Structure

```
.
├── index.html   # markup and content
├── style.css    # styling, themes, animations
└── README.md
```

## Notes

Fonts are loaded from Google Fonts, so an internet connection is needed for them to appear. Offline, the page falls back to system fonts.
