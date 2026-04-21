# Core Web Vitals Guide

Understanding and optimizing Core Web Vitals for better rankings and user experience.

## What Are Core Web Vitals?

Core Web Vitals are three specific metrics Google uses to measure user experience:

1. **LCP (Largest Contentful Paint)** — Loading performance
2. **FID (First Input Delay)** / **INP (Interaction to Next Paint)** — Interactivity
3. **CLS (Cumulative Layout Shift)** — Visual stability

## Metric Thresholds

### LCP (Largest Contentful Paint)
- **Good:** ≤ 2.5 seconds
- **Needs Improvement:** 2.5 - 4.0 seconds
- **Poor:** > 4.0 seconds

**What it measures:** Time for the largest visible content element (image or text block) to render.

### FID (First Input Delay) → INP (Interaction to Next Paint)
- **Good:** ≤ 100ms (FID) / ≤ 200ms (INP)
- **Needs Improvement:** 100-300ms (FID) / 200-500ms (INP)
- **Poor:** > 300ms (FID) / > 500ms (INP)

**What it measures:** Time from user interaction (click, tap) to browser response. INP replaces FID in 2024.

### CLS (Cumulative Layout Shift)
- **Good:** ≤ 0.1
- **Needs Improvement:** 0.1 - 0.25
- **Poor:** > 0.25

**What it measures:** Unexpected layout shifts during page load (elements moving around).

## How to Measure

### Field Data (Real Users)
- **Chrome User Experience Report (CrUX)** — GSC Core Web Vitals report
- **Google Analytics 4** — Web Vitals events
- **RUM tools** — Cloudflare, SpeedCurve, etc.

### Lab Data (Controlled Tests)
- **PageSpeed Insights**
- **Lighthouse**
- **WebPageTest**
- **GTmetrix**

**Note:** Field data is what counts for rankings, but lab data helps debug.

## LCP Optimization

### Common LCP Elements
1. Hero image
2. Large text block (H1)
3. Background image
4. Video poster image

### LCP Fixes

**1. Optimize Images**
```html
<!-- Use responsive images -->
<picture>
  <source srcset="hero.webp" type="image/webp">
  <source srcset="hero.jpg" type="image/jpeg">
  <img src="hero.jpg" alt="Description" width="1200" height="800">
</picture>
```

**2. Preload Critical Resources**
```html
<link rel="preload" as="image" href="/hero-image.webp" fetchpriority="high">
```

**3. Server Response Time**
- Use a fast host/CDN
- Enable caching
- Optimize database queries
- Use edge functions for dynamic content

**4. Remove Render-Blocking Resources**
- Inline critical CSS
- Defer non-critical JavaScript
- Load fonts with `font-display: swap`

### LCP Quick Wins
- [ ] Compress hero images (TinyPNG, Squoosh)
- [ ] Serve images in WebP/AVIF format
- [ ] Add explicit width/height attributes to images
- [ ] Use a CDN (Cloudflare, CloudFront)
- [ ] Preload LCP image

## FID/INP Optimization

### Common Culprits
1. Heavy JavaScript execution
2. Third-party scripts (analytics, ads, widgets)
3. Large JavaScript bundles
4. Main thread blocking

### FID/INP Fixes

**1. Break Up Long Tasks**
```javascript
// BAD: Blocks for 1 second
function heavyTask() {
  // Do 1 second of work
}

// GOOD: Yield to main thread
async function heavyTask() {
  for (let i = 0; i < 10; i++) {
    await new Promise(r => requestIdleCallback(r));
    // Do 100ms of work
  }
}
```

**2. Defer Non-Critical JavaScript**
```html
<script src="analytics.js" defer></script>
<script src="ads.js" async></script>
```

**3. Lazy Load Third-Party Scripts**
```javascript
// Load only when needed
const chatWidget = document.querySelector('#chat');
const observer = new IntersectionObserver((entries) => {
  if (entries[0].isIntersecting) {
    loadChatScript();
  }
});
observer.observe(chatWidget);
```

**4. Web Workers for Heavy Processing**
```javascript
// Offload work from main thread
const worker = new Worker('worker.js');
worker.postMessage({ action: 'process', data: largeData });
```

### FID/INP Quick Wins
- [ ] Defer JavaScript
- [ ] Remove unused JavaScript
- [ ] Code-split with dynamic imports
- [ ] Minimize third-party scripts
- [ ] Use requestAnimationFrame for visual updates

## CLS Optimization

### Common CLS Culprits
1. Images without dimensions
2. Ads/embeds without reserved space
3. Web fonts causing FOUT/FOIT
4. Content injected dynamically
5. Cookie banners shifting content

### CLS Fixes

**1. Set Image Dimensions**
```html
<!-- Always include width/height -->
<img src="photo.jpg" width="800" height="600" alt="Description">

<!-- Or use aspect ratio via CSS -->
<img src="photo.jpg" style="aspect-ratio: 4/3;" alt="Description">
```

**2. Reserve Space for Ads/Embeds**
```css
.ad-container {
  min-height: 250px;
  /* Or use aspect-ratio for responsive */
  aspect-ratio: 16 / 9;
}
```

**3. Preload Fonts**
```html
<link rel="preload" href="font.woff2" as="font" type="font/woff2" crossorigin>
```

**4. Use font-display: swap**
```css
@font-face {
  font-family: 'CustomFont';
  src: url('font.woff2') format('woff2');
  font-display: swap;
}
```

**5. Don't Insert Content Above Existing Content**
```css
/* BAD: Inserting at top of body */
.notification {
  position: fixed;
  top: 0;
  /* Reserve space or use overlay */
}

/* GOOD: Reserve space in layout */
.header {
  margin-top: 50px; /* Space for notification */
}
```

### CLS Quick Wins
- [ ] Add width/height to all images
- [ ] Reserve space for ads/iframes
- [ ] Use font-display: swap for custom fonts
- [ ] Preload above-the-fold fonts
- [ ] Don't insert cookie banners at top (use bottom or overlay)

## Advanced Optimizations

### Resource Hints
```html
<!-- Preconnect to third-party domains -->
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<!-- Prefetch likely next page -->
<link rel="prefetch" href="/next-page.html">

<!-- Preload critical resources -->
<link rel="preload" href="/critical.css" as="style">
```

### HTTP/2 and HTTP/3
- Enable HTTP/2 push (deprecated but still useful)
- Use HTTP/3 if available (better for mobile)

### CDN Configuration
- Cache static assets aggressively
- Use edge caching for HTML
- Optimize TLS configuration

### Image Optimization Service
Consider services like:
- Cloudflare Image Resizing
- Cloudinary
- Imgix
- Sanity image pipeline

## Monitoring

### Set Up Alerts
- GSC Core Web Vitals report — check monthly
- PageSpeed Insights API — weekly automated checks
- Real User Monitoring (RUM) — continuous

### Reporting Template
| Metric | Target | Current | Status | Action |
|--------|--------|---------|--------|--------|
| LCP | < 2.5s | 2.1s | ✅ Good | Monitor |
| INP | < 200ms | 320ms | ⚠️ Needs Work | Defer JS |
| CLS | < 0.1 | 0.15 | ⚠️ Needs Work | Image dimensions |

## Common Issues by Platform

### WordPress
- Too many plugins
- Heavy themes
- Render-blocking resources

**Fixes:**
- Use caching plugin (WP Rocket, LiteSpeed)
- Optimize images with plugin
- Lazy load videos/iframes

### Shopify
- Third-party apps
- Heavy themes
- Product images not optimized

**Fixes:**
- Compress product images before upload
- Limit apps
- Use Shopify's CDN

### Custom/JAMstack
- JavaScript bundle size
- Client-side rendering
- Large assets

**Fixes:**
- Static generation where possible
- Code splitting
- Edge caching

### Photography Sites
- Large hero images
- Galleries without optimization
- Lightbox libraries

**Fixes:**
- Compress images (TinyPNG, Squoosh)
- Use WebP
- Lazy load galleries
- Implement responsive images (srcset)

## Testing Checklist

Before and after optimizations:

- [ ] Test on mobile (throttled 3G)
- [ ] Test on desktop (cable connection)
- [ ] Test with and without cache
- [ ] Test logged in vs logged out
- [ ] Test different browsers
- [ ] Test with ad blockers off
- [ ] Verify field data improves (wait 28 days after changes)

## Tools Summary

| Tool | Best For |
|------|----------|
| PageSpeed Insights | Quick checks, field data |
| Lighthouse | Detailed analysis, CI/CD |
| WebPageTest | Deep diagnostics, filmstrip |
| GTmetrix | Trending, alerts |
| Chrome DevTools | Live debugging |
| CrUX Dashboard | BigQuery analysis |
| GSC | Real user field data |
