## 2025-01-31 - [Deferring Third-Party Embeds]
**Learning:** Third-party embeds like Google Maps (even with `loading="lazy"`) can still trigger a significant number of requests and data transfer if they are within or near the initial viewport. Replacing them with a "Click-to-load" placeholder is a far more effective optimization for improving initial load performance (LCP/TBT).
**Action:** Always check for heavy third-party iframes and consider if they can be deferred until user interaction, especially if they are not critical for the initial page view.
