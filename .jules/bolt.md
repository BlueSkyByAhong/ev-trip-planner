## 2025-05-15 - Deferring Google Maps with Click-to-load
**Learning:** Deferring heavy third-party embeds (like Google Maps) using a 'Click-to-load' pattern is a highly effective optimization for this project, significantly reducing initial page load weight and requests. This is especially useful for mobile users or those on slower connections who may not need the map immediately.
**Action:** Always check for heavy iframes or third-party scripts that can be deferred until user interaction.

## 2025-05-16 - Verifying CSS Before Adding Image Dimensions
**Learning:** When adding explicit width and height to images to prevent CLS, it is critical to verify the current CSS rules first. If the CSS defines a different size or aspect ratio than the attributes, it could cause layout regressions or image distortion.
**Action:** Always grep for the image class or parent container in the CSS before assigning hardcoded dimensions to <img> tags.
