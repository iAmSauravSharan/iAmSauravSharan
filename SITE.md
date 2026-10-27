# Portfolio site (Astro)

Rebuilt from a saved copy of carterogunsola.com. All copy, names, links and images are the original placeholders and are kept as-is on purpose.

- `src/pages/index.astro` renders `src/content/home.html` (the saved page markup, with asset paths rewritten to `/assets`, `/fonts`, `/og`).
- `public/` holds the CSS, fonts, favicons and manifest from the export.
- `npm run dev` / `npm run build` / `npm run preview`.

## Known gaps in the export
- The site's interactive JavaScript bundles were left out: the saved copy only had 3 of their many chunks, so they would 404. The page is static (no WebGL paper/shelf effects, live clock, page transitions). The loading overlay clears itself after about 4 seconds via a CSS fallback.
- The original Cloudflare analytics beacon was removed.
- Not in the export, so they still 404: `/media/plates/*` client logos, `/icon-192.png`, `/icon-512.png`, and the sub-pages (`/about`, `/lab`, `/writing`, `/studio`, `/contact`, ...).
