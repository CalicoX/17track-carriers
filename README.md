# 17TRACK Carriers — DHL Express

A 17TRACK carrier landing page for DHL Express tracking, built as static HTML and CSS.

## Structure

```
index.html          Carrier page markup
styles.css          Compiled stylesheet (linked by the page)
src/styles.scss     SCSS source
bfcm/               Logo and header icon assets (SVG)
figma/              Icon assets (SVG)
footer/             Footer logos, social icons, store badges
favicon.svg         Favicon
dhl.webp            Carrier logo
dhl-express.webp    Carrier logo (alternate)
```

## Local preview

Serve the directory over HTTP (any static server works):

```bash
python3 -m http.server 8800 --bind 127.0.0.1
```

Then open <http://127.0.0.1:8800/>.

## Styling notes

`styles.css` is the file the page loads. `src/styles.scss` is the readable source and is kept in sync
manually — edits belong in both files.

Brand colors follow the 17TRACK logo: blue `#003a9b`, orange `#ff8c00`.

The "Advance features" buttons (`Auto-import`, `Tracking API`) use a white card with a solid brand-colored
icon tile and a white glyph. They intentionally have no gradient and no hover shadow.

## Responsive behavior

- Buttons: one per row at ≤640px; two per row from 641px up (including iPad).
- The tracking input keeps the multi-line list layout at every breakpoint.
