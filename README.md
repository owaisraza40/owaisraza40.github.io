# Owais Raza — Portfolio (V6)

Same sage/cream editorial direction as before, with a full pass to fix what was
undermining it:

**Fixed**
- Contrast failure on the small red-tile labels (was 4.2:1, now 6.67:1 — passes WCAG AA)
- `-webkit-text-stroke` on the hero headline had no fallback — on unsupported
  browsers the word "LEARN" rendered fully invisible. Now falls back to solid ink text.
- No visible keyboard focus state anywhere — added `:focus-visible` outlines site-wide
- No `prefers-reduced-motion` support — added
- The Hasteel Elevators tile was nearly invisible against the page background
  (measured 1.09:1) — now has real texture and border definition
- Smallest text sizes (7px/8px on mobile) bumped to a 10–11px floor for legibility

**Replaced**
- The generic circle/card/dot/cross hero illustration → a real "status card" with
  actual info (stack, base, focus, availability, latest ship) instead of decorative filler text
- Meaningless decorative numbering (a "07" watermark, "SERIES 01," numbered
  section/project tags) → dropped, or replaced with labels that mean something
  ("LIVE · CLIENT SITE" instead of "03")
- Bare 2-letter project monograms (AN / RA / HE / PF) → small custom icons specific
  to each project (a flight path for AeroNexus, sentiment bars for Review Analysis,
  an elevator shaft for Hasteel, code brackets for Programming Fundamentals)

**Added**
- Open Graph / Twitter card meta tags + `og-image.png` so the link shows a real
  preview card when shared
- An inline SVG favicon
- A skip-to-content link
- A dynamic copyright year (no longer hardcoded)

## Publish

Upload `index.html`, `style.css`, `script.js`, `og-image.png`, and `README.md` to
the root of the `main` branch in `owaisraza40.github.io`, replacing everything
currently there.

In GitHub: **Settings → Pages → Deploy from a branch → `main` → `/(root)`**

**Before publishing:** open `index.html`, search for `REPLACE-WITH`, and swap in
your real LinkedIn URL and email (contact section, near the bottom). Marked with
an HTML comment so it's easy to find.
