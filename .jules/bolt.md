## 2025-05-15 - Deferring Google Maps with Click-to-load
**Learning:** Deferring heavy third-party embeds (like Google Maps) using a 'Click-to-load' pattern is a highly effective optimization for this project, significantly reducing initial page load weight and requests. This is especially useful for mobile users or those on slower connections who may not need the map immediately.
**Action:** Always check for heavy iframes or third-party scripts that can be deferred until user interaction.

## 2025-05-16 - Cumulative Layout Shift (CLS) Mitigation
**Learning:** Adding explicit `width` and `height` attributes to `<img>` tags, even when CSS also specifies them, allows the browser to allocate space for the image during the initial HTML parse. This prevents layout jumps (CLS) as images load or when CSS is applied. Correcting malformed viewport meta tags is also critical for mobile rendering performance.
**Action:** Always ensure `<img>` tags have dimensions and use `decoding="async"` to keep the main thread responsive. Fix viewport tags to use standard `initial-scale=1.0` syntax.
