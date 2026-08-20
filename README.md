# Chichi's Bouquet

A single-page birthday card. A hand-tied bouquet sways on a dark botanical
ground; tap it and the wrapping falls open, the flower heads scatter into a
petal burst, and the wish rises behind them.

**Live:** https://shivankj379.github.io/happy-birthday-chichi/

## Editing

Everything you'd want to change lives in the `WISH` object near the top of the
`<script>` block in `index.html` — the name, the opening line, the message and
the signature.

Non-ASCII characters are written as escapes (`—`, `\u{1FAF6}`) so the page
can't break on a host that forgets to send `charset=utf-8`.

## Notes

`index.html` is fully self-contained — no build step, no dependencies, no local
asset files. The photo is embedded as a base64 data URI and the bouquet is drawn
parametrically in SVG at runtime. The only external request is Google Fonts.

To preview locally:

    python3 -m http.server 4321
