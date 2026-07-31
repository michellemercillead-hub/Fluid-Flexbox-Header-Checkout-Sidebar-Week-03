Fluid Flexbox Header & Checkout Sidebar
=====================================

Project overview
----------------
A small demo layout showcasing a multi-tier responsive header and a checkout page with a form area and a sidebar summary. The stylesheet uses modern CSS practices: global `box-sizing: border-box`, CSS logical properties (`padding-block`, `padding-inline`, `margin-block`, `margin-inline`), and Flexbox with `gap` for spacing.

Key features
------------
- Multi-tier header (utility bar + main nav) that keeps items vertically centered and spaced using Flexbox and `gap`.
- Checkout layout with a form container and an adjacent order summary sidebar on wide viewports; stacks on narrow screens.
- Logical properties only for box model adjustments to support RTL and different writing modes.
- Global `box-sizing: border-box` and careful use of `inline-size` / `block-size` where appropriate.

Files
-----
- `index.html` — markup for header and checkout layout.
- `styles.css` — modern stylesheet using logical properties and Flexbox.

Preview locally
---------------
Open `index.html` in your browser. For a quick local server (recommended for images/paths), run in the project folder:

```bash
# Python 3 (simple HTTP server)
python -m http.server 8000
# then open http://localhost:8000 in your browser
```

Notes
-----
- The CSS intentionally avoids physical directional properties (`margin-left`, `padding-top`, etc.) in favor of logical properties for better internationalization and more predictable layout.
- `gap` is used on flex containers for consistent spacing between items. This is supported in modern browsers.

Credits
-------
This README (and parts of the stylesheet) were created with assistance from an AI to speed up authoring and ensure modern best practices were applied.

If you want, I can:
- Add a quick visual screenshot.
- Add browser-compatibility notes or a small CSS fallback for older browsers (IE11).
- Convert the project into a tiny dev server workflow (npm + live-server).
