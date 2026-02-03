## 2025-05-15 - Deferring Google Maps with Click-to-load
**Learning:** Deferring heavy third-party embeds (like Google Maps) using a 'Click-to-load' pattern is a highly effective optimization for this project, significantly reducing initial page load weight and requests. This is especially useful for mobile users or those on slower connections who may not need the map immediately.
**Action:** Always check for heavy iframes or third-party scripts that can be deferred until user interaction.

## 2025-05-16 - Explicit Image Dimensions and Viewport Fixes
**Learning:** Even with `loading="lazy"`, missing `width` and `height` attributes on images cause Cumulative Layout Shift (CLS) as the browser cannot reserve space. Additionally, a typo in the viewport meta tag (`initial-scale-1.0` vs `initial-scale=1.0`) can break mobile rendering and impact perceived performance.
**Action:** Always ensure `width` and `height` are set for all images, and double-check meta tag syntax for critical SEO and performance tags. Use `decoding="async"` for non-critical images to keep the main thread clear.
