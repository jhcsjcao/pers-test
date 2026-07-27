# Project Conventions

## `uver` — Cache-bust version bump

When the user types `uver`, increment the service worker cache version in `pwa/sw.js` by `0.01`.

**Pattern:** `ocean-assessment-vX.YY.ZZ`

**Examples:**
- `v1.00.02` → `v1.00.03`
- `v1.00.09` → `v1.00.10`
- `v1.99.99` → `v2.00.00`

Always change all three:
1. The `const CACHE = 'ocean-assessment-v...'` line in `pwa/sw.js`
2. The version badge `<div>vX.YY.ZZ</div>` on the landing page in `pwa/index.html`
3. The `sw.js?v=X.YY.ZZ` query param in the SW registration at the bottom of `pwa/index.html`
