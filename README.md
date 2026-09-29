# The Quiet Strength: ebook website

A single-page promo site for *The Quiet Strength: How to Rebuild Confidence, Find Direction, and Move Forward When Life Changes* by Ashwik Bire.

Buy link: https://amzn.in/d/0elSxaV1

## What's inside

| File | Purpose |
| --- | --- |
| `quiet-strength.html` | The whole site: HTML, CSS, JavaScript and the cover image (embedded) in one file |
| `README.md` | This guide |

## Page sections

1. **Hero:** headline, subtitle, author name, cover and Amazon button
2. **Moments:** the situations the book is written for
3. **Frameworks:** tabs for the Circle of Control, Action Ladder, Mistake Recovery Framework and Life Audit
4. **Inside the book:** all seven chapters with a one-line summary each
5. **Quote and call to action**
6. **Footer:** copyright and disclaimer

## Run it locally

Open `quiet-strength.html` in any browser. No build step or dependencies are needed. Fonts (Poppins and Lora) load from Google Fonts, so an internet connection is needed to see them; otherwise the page falls back to system fonts.

## Deploy

Rename the file to `index.html` if your host expects that, then upload it to any static host:

- **GitHub Pages:** put `index.html` in a repository, then enable Pages in Settings.
- **Netlify or Vercel:** drag and drop the file or folder.
- **Any web server:** copy the file to the site's public folder.

## Customize

- **Colors and fonts:** edit the CSS variables at the top of the `<style>` block (`--bg`, `--moss`, `--copper`, `--head`, `--body`). Dark mode has its own set of variables in the same place.
- **Buy link:** search for `amzn.in/d/0elSxaV1` and replace every match.
- **Cover image:** the cover is embedded as a base64 `data:` URI in the `<img>` tag. To use a separate file instead, replace the `src` value with a path such as `cover.jpg`.
- **Chapter summaries and framework text:** edit the HTML directly. Each is plain markup.

## Open Graph and sharing

The `<head>` includes these Open Graph tags:

- `og:site_name`
- `og:title`
- `og:type`
- `og:description`
- `og:locale`
- `book:author`

To get a preview image and canonical link when the page is shared, add these two tags once the site is live:

```html
<meta property="og:url" content="https://your-domain.com/">
<meta property="og:image" content="https://your-domain.com/cover.jpg">
```

Both must be absolute URLs, and the image file has to be hosted separately (about 1200 x 630 px works best for previews).

## Accessibility

- Keyboard-navigable framework tabs (arrow keys switch tabs)
- Visible focus outlines
- Light and dark themes that follow the system setting
- Reduced-motion preference respected
- Responsive from phone to desktop

## Copyright

&copy; 2026 Ashwik Bire. All rights reserved. First edition.

This book is for education and reflection. It does not provide medical, psychological, financial or legal advice.
