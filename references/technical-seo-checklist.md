# Technical SEO Checklist

Complete technical SEO audit checklist for crawling, indexing, and site architecture.

## Crawlability

### Robots.txt
- [ ] File exists at domain root
- [ ] No accidental blocking of important content
- [ ] XML sitemap referenced
- [ ] No syntax errors
- [ ] User-agent specific rules correct

**Common robots.txt issues:**
```
# BAD - blocks entire site
User-agent: *
Disallow: /

# BAD - blocks CSS/JS (Google needs these)
Disallow: /css/
Disallow: /js/

# GOOD
User-agent: *
Disallow: /admin/
Disallow: /cart/
Sitemap: https://example.com/sitemap.xml
```

### XML Sitemap
- [ ] Accessible at /sitemap.xml or /sitemap_index.xml
- [ ] Valid XML format (test at xml-sitemaps.com/validate-xml-sitemap.html)
- [ ] Under 50,000 URLs or 50MB
- [ ] Only includes canonical, indexable URLs
- [ ] No 404s or redirects in sitemap
- [ ] Lastmod dates updated
- [ ] Submitted in Google Search Console

### Crawl Budget Optimization
- [ ] Low-value pages noindexed (pagination, filters, sort)
- [ ] Orphan pages identified and linked
- [ ] Redirect chains minimized
- [ ] 404s fixed or properly handled

## Indexing

### Meta Robots
- [ ] No accidental noindex on important pages
- [ ] Noindex applied to thin/low-value pages
- [ ] Nofollow used appropriately
- [ ] X-Robots-Tag headers checked for PDFs, etc.

**Patterns:**
```html
<!-- Index, follow (default) -->
<meta name="robots" content="index, follow">

<!-- Noindex -->
<meta name="robots" content="noindex">

<!-- Noindex, nofollow -->
<meta name="robots" content="noindex, nofollow">
```

### Canonical Tags
- [ ] Self-referencing canonicals on all pages
- [ ] Cross-domain canonicals for syndicated content
- [ ] No conflicting signals (canonical vs noindex)
- [ ] Canonicals point to HTTPS versions
- [ ] Trailing slash consistency

**Examples:**
```html
<!-- Self-referencing -->
<link rel="canonical" href="https://example.com/page/">

<!-- With parameters -->
<link rel="canonical" href="https://example.com/products/">
<!-- NOT: https://example.com/products?sort=price -->
```

## URL Structure

### Best Practices
- [ ] Short URLs (under 60 characters)
- [ ] Hyphens between words (not underscores)
- [ ] Lowercase only
- [ ] No special characters (&, %, $)
- [ ] No session IDs or parameters
- [ ] No file extensions (.html, .php) if possible

**Examples:**
```
GOOD:  /wedding-photography/toronto/
BAD:   /wedding_photography_toronto.html
BAD:   /index.php?page=wedding&id=123
BAD:   /Wedding-Photography/
```

### URL Consistency
- [ ] Trailing slash policy enforced (all URLs end with / or none)
- [ ] WWW vs non-WWW redirect properly
- [ ] HTTPS enforced (301 from HTTP)
- [ ] No mixed case

## Status Codes

### 200 OK
- [ ] All important pages return 200
- [ ] No soft 404s (page shows "not found" but returns 200)

### 301 Redirects
- [ ] Old URLs redirect to new versions
- [ ] Redirect chains < 3 hops
- [ ] No redirect loops

### 404 Not Found
- [ ] Custom 404 page helpful and branded
- [ ] 404 page returns actual 404 status
- [ ] Broken internal links fixed or removed

### Other Status Codes
- [ ] 410 used for permanently removed content (optional)
- [ ] 503 for maintenance mode (if applicable)

## Site Architecture

### Click Depth
- [ ] Important pages within 3 clicks of homepage
- [ ] Orphan pages identified and linked
- [ ] Flat architecture when possible

### Internal Linking
- [ ] Every page has at least one internal link
- [ ] Contextual links in content
- [ ] Navigation links logical
- [ ] Footer links helpful

### Pagination
- [ ] Rel="next" and rel="prev" (deprecated but still used)
- [ ] View-all page canonical preferred (if exists)
- [ ] Infinite scroll has fallback pagination

### Faceted Navigation (E-commerce)
- [ ] Parameters handled (robots.txt or canonical)
- [ ] No crawl bloat from filter combinations
- [ ] Important facets have dedicated pages

## JavaScript SEO

### Rendering
- [ ] Google can render JavaScript content
- [ ] Key content not hidden behind JS interactions
- [ ] Lazy loading implemented correctly
- [ ] No critical content in JS that fails

### Testing
Test with:
- Google Search Console URL Inspection → View Crawled Page
- Mobile-Friendly Test
- Screaming Frog JavaScript rendering mode

## Site Speed

### Server Response
- [ ] TTFB < 200ms
- [ ] Server supports HTTP/2
- [ ] Compression enabled (Gzip/Brotli)
- [ ] CDN used for static assets

### Resource Loading
- [ ] CSS not render-blocking (or minified)
- [ ] JS deferred/async where possible
- [ ] Preconnect hints for third-party domains
- [ ] Prefetch DNS for anticipated resources

### Caching
- [ ] Browser caching enabled
- [ ] Cache headers set appropriately
- [ ] ETags configured
- [ ] Service Worker for PWA (optional)

## Mobile-First Indexing

### Mobile Parity
- [ ] Mobile and desktop content identical
- [ ] No mobile-specific cloaking
- [ ] Structured data present on mobile
- [ ] Internal links identical on mobile

### Responsive Design
- [ ] Viewport meta tag present
- [ ] No fixed-width elements causing horizontal scroll
- [ ] Font size readable without zoom
- [ ] Tap targets > 48x48px

## International SEO

### Hreflang
- [ ] Tags on all language/region variants
- [ ] Self-referencing hreflang on each page
- [ ] x-default specified
- [ ] Bi-directional (en links to fr, fr links to en)
- [ ] No conflicting canonicals

**Example:**
```html
<link rel="alternate" hreflang="en-us" href="https://example.com/en-us/" />
<link rel="alternate" hreflang="en-gb" href="https://example.com/en-gb/" />
<link rel="alternate" hreflang="en" href="https://example.com/en/" />
<link rel="alternate" hreflang="x-default" href="https://example.com/" />
```

### Language Signals
- [ ] HTML lang attribute correct
- [ ] Currency and units appropriate
- [ ] Local phone numbers and addresses

## Security

### HTTPS
- [ ] SSL certificate valid and not expiring soon
- [ ] All pages redirect HTTP → HTTPS
- [ ] HSTS header present
- [ ] Mixed content resolved (no HTTP resources on HTTPS)

**Mixed content check:**
```
Browser console: "Mixed Content: The page at..."
```

### Security Headers
- [ ] Content-Security-Policy
- [ ] X-Frame-Options
- [ ] X-Content-Type-Options
- [ ] Referrer-Policy

## Structured Data

### Implementation
- [ ] JSON-LD format preferred
- [ ] Validated with Google's Rich Results Test
- [ ] No errors or warnings
- [ ] Not misleading or inaccurate

### Required Types
- [ ] Organization on homepage
- [ ] WebSite for site search box
- [ ] BreadcrumbList on all pages
- [ ] LocalBusiness (if applicable)
- [ ] Service/Product pages marked up

## Log File Analysis

### What to Check
- [ ] Crawl frequency by Googlebot
- [ ] Pages never crawled
- [ ] 5xx errors seen by bots
- [ ] JavaScript resources blocked
- [ ] Crawl budget waste (low-value pages crawled often)

**Tools:** Screaming Frog Log Analyzer, Splunk, custom scripts

## Common Technical Issues

| Issue | Impact | How to Find |
|-------|--------|-------------|
| Orphan pages | Not indexed | Screaming Frog crawl + GA/GSC data |
| Redirect chains | Lost link equity, slow | Screaming Frog |
| Duplicate content | Cannibalization | Siteliner, Screaming Frog |
| 404 errors | Bad UX, wasted crawl | GSC Coverage report |
| Thin content | Poor rankings | GA bounce rate + word count analysis |
| Slow TTFB | Ranking factor | PageSpeed Insights, GTmetrix |
| Mobile issues | Mobile-first indexing | GSC Mobile Usability |
