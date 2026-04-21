---
name: seo-audit
description: "Conduct comprehensive SEO audits: technical SEO, on-page analysis, local SEO, content audits, backlink analysis, and competitor research. Produces a structured report with health score, priorities, and actionable improvements. Works for photographers, creatives, consultants, e-commerce, and small businesses."
---

# Comprehensive SEO Audit Skill

> **Version**: 1.0 | **Platform**: OpenClaw (adaptable to any AI agent)

Systematically analyze website SEO performance and produce actionable improvement plans.

---

## When to Use

- Full SEO audit for any website
- Diagnosing traffic drops or ranking declines
- Pre-redesign or migration SEO review
- Competitive gap analysis
- Quick win identification
- Creating SEO roadmaps and strategies

---

## Before You Start

Gather:
- **Target website URL**
- **Primary business goals** (leads, sales, brand awareness)
- **Target audience** (who searches, why)
- **2-5 direct competitors** (businesses targeting same audience)
- **Geographic focus** (local, regional, national, global)

---

## The Audit Framework

### Phase 1 — Discovery

**Define the audit scope:**
1. What type of website? (photographer, e-commerce, blog, service business)
2. What are the top 3 business goals the website supports?
3. Who is the primary search audience?
4. What search intent matters most? (informational, transactional, local)

**Identify competitors:**
List 2-5 businesses that:
- Rank for your target keywords
- Serve the same audience
- Are aspirational benchmarks

---

### Phase 2 — Technical SEO Audit

Run these checks using PageSpeed Insights, Screaming Frog, or manual testing:

#### Crawlability
- [ ] Robots.txt exists and doesn't block important content
- [ ] XML sitemap submitted to Google Search Console
- [ ] Canonical tags correctly implemented
- [ ] No accidental noindex on key pages
- [ ] No redirect chains (A→B→C)
- [ ] 404s return proper 404 page (not soft 404)

#### Site Architecture
- [ ] All important pages within 3 clicks of homepage
- [ ] No orphan pages (pages with no internal links)
- [ ] Logical URL structure (short, descriptive, hyphens)
- [ ] HTTPS enabled sitewide
- [ ] No mixed content errors (HTTP resources on HTTPS page)

#### Mobile
- [ ] Responsive design (test with Chrome DevTools device toolbar)
- [ ] Mobile viewport properly configured
- [ ] No horizontal scrolling on mobile
- [ ] Tap targets appropriately sized

#### Core Web Vitals
| Metric | Good | Needs Work | Poor |
|--------|------|-----------|------|
| LCP | < 2.5s | 2.5-4s | > 4s |
| FID/INP | < 100ms | 100-300ms | > 300ms |
| CLS | < 0.1 | 0.1-0.25 | > 0.25 |

**Fix priorities:**
- LCP > 2.5s: Optimize images (compress, WebP), reduce server response time
- CLS > 0.1: Set image dimensions, avoid layout shifts from ads/fonts
- INP > 200ms: Reduce JavaScript execution time

#### Security
- [ ] HTTPS enabled on all pages
- [ ] No mixed content warnings
- [ ] Security headers present (X-Frame-Options, CSP)

---

### Phase 3 — On-Page SEO Audit

#### Title Tags
- [ ] Unique per page (no duplicates)
- [ ] 50-60 characters
- [ ] Primary keyword near the start
- [ ] Brand name included (except homepage)
- [ ] Compelling (not just keyword list)

**Check**: View page source or use Screaming Frog to see all titles at once.

#### Meta Descriptions
- [ ] Unique per page
- [ ] 150-160 characters
- [ ] Primary + secondary keyword included
- [ ] Soft CTA (e.g., "Learn more", "Get a quote")
- [ ] Click-worthy copy (not generic)

#### Headings (H1-H6)
- [ ] Exactly one H1 per page
- [ ] H1 contains primary keyword
- [ ] Logical H2-H6 hierarchy (no skips: H1→H3)
- [ ] Keywords used naturally in headings
- [ ] No heading spam (keyword stuffing)

#### Content Quality
- [ ] Minimum 300 words on standard pages
- [ ] Primary keyword in first 100 words
- [ ] Related/LSi keywords used naturally
- [ ] No duplicate content (internal or external)
- [ ] E-E-A-T signals present (credentials, experience, references)
- [ ] Content updated recently (check lastmod dates)

**E-E-A-T Checklist:**
- Expertise: Author credentials visible?
- Experience: First-hand experience demonstrated?
- Authoritativeness: Backed by credentials, reviews, references?
- Trustworthiness: Accurate, honest, no red flags?

#### Image Optimization
- [ ] Descriptive file names (e.g., `wedding-photography-venue-name.jpg` not `IMG_1234.jpg`)
- [ ] Alt text present on all images (under 125 characters)
- [ ] Images compressed (< 200KB per image ideal)
- [ ] WebP format used where supported
- [ ] Width/height attributes set to prevent CLS

#### Schema Markup (JSON-LD)
- [ ] Organization schema on homepage
- [ ] LocalBusiness schema (if local business)
- [ ] Service schema (for service pages)
- [ ] FAQ schema (for FAQ pages)
- [ ] Review/aggregateRating schema (for pages with reviews)
- [ ] BreadcrumbList schema

**Verify**: Use Google's Rich Results Test (search.google.com/test/rich-results)

#### Internal Linking
- [ ] Contextual links within content (not just nav)
- [ ] Anchor text descriptive (not "click here")
- [ ] Priority pages linked from homepage
- [ ] No broken internal links

#### URL Structure
- [ ] Short and readable (under 75 characters)
- [ ] Hyphens between words (not underscores)
- [ ] Lowercase only
- [ ] No parameters or session IDs
- [ ] No special characters

---

### Phase 4 — Local SEO Audit (if applicable)

#### Google Business Profile (GBP)
- [ ] Profile claimed and verified
- [ ] NAP (Name, Address, Phone) matches website exactly
- [ ] Primary category correctly selected
- [ ] Secondary categories added
- [ ] Photos uploaded (exterior, interior, team, portfolio samples)
- [ ] Posts/updates published regularly
- [ ] Q&A populated (seed with common questions)
- [ ] Reviews responded to (never ignore negative reviews)
- [ ] 5+ reviews with high rating (aim for 4.5+)

#### Local Citations
- [ ] NAP consistent across: Yelp, Bing Places, Apple Maps, Facebook
- [ ] Industry-specific directories (wedding photographer → WeddingWire, The Knot)
- [ ] No duplicate listings
- [ ] Data aggregator submissions (Neustar/Localeze, Foursquare)

**Check**: Use BrightLocal, Whitespark, or Yext for citation audit.

#### On-Site Local Signals
- [ ] NAP in website footer (every page)
- [ ] NAP on contact page
- [ ] Embedded Google Map on contact page
- [ ] Location-specific content (neighborhood guides, area photography)
- [ ] Local keywords used naturally (city, neighborhood names)

---

### Phase 5 — Content Audit

**Create a content inventory:**
List every page and score it on:
- Organic traffic (from GSC)
- Conversions (leads, sales, sign-ups)
- Bounce rate
- Time on page
- Current keyword rankings

**Classify each page:**
| Type | Action |
|------|--------|
| High traffic + high conversions | Protect and improve |
| High traffic + low conversions | Investigate and fix |
| Low traffic + high conversions | Expand / promote |
| Low traffic + low conversions | Improve, consolidate, or remove |

**Content gaps:**
- What do competitors rank for that you don't?
- What questions does your audience ask that you haven't answered?
- What topics have search volume but no content?

---

### Phase 6 — Backlink Audit

**Gather data from:** Ahrefs, Moz, Google Search Console, or Ubersuggest

**Profile overview:**
- Total referring domains
- Domain Rating / Authority distribution
- Follow vs. nofollow ratio (aim for 60-80% dofollow)
- Link velocity (new links per month)

**Link quality check:**
- [ ] No toxic links (link farms, PBNs, spam)
- [ ] Anchor text not over-optimized
- [ ] Link diversity (not all from one source)
- [ ] No links from irrelevant websites

**Reclamation opportunities:**
- [ ] Pages that returned 404 with valuable backlinks → set up redirects
- [ ] Unlinked brand mentions → reach out for link

---

### Phase 7 — Competitor Analysis

**Identify competitors:**
- Who ranks on page 1 for your target keywords?
- Who appears in the "People also ask" box?
- Who shows up in the local map pack?

**Benchmark matrix:**
| Metric | Your Site | Competitor 1 | Competitor 2 |
|--------|-----------|--------------|--------------|
| Domain Rating | | | |
| Organic Traffic Est. | | | |
| Referring Domains | | | |
| Top 5 Ranking Keywords | | | |
| Content Volume | | | |
| Core Web Vitals Status | | | |
| Local SEO Score | | | |

**Gap analysis:**
- Keywords they rank for that you don't
- Content formats they use (video, tools, guides)
- Features they have that you don't
- Backlink sources you could replicate

---

## Audit Output

Structure the final report:

### 1. Executive Summary (1-2 pages)
- **Health Score**: 0-100 (weight: Technical 30%, On-page 25%, Content 20%, Backlinks 15%, Local 10%)
- **Top 3 Priorities**: Must-fix items with highest impact
- **Quick Wins**: High impact, low effort fixes
- **Resource Estimate**: Hours and tools needed

### 2. Technical SEO Report
- Issues found with severity (Critical / High / Medium / Low)
- Specific fix instructions
- Estimated effort per fix

### 3. On-Page SEO Report
- Per-page issues (title, meta, content, images)
- Priority pages first (homepage, service pages, top-traffic pages)

### 4. Local SEO Report
- GBP optimization status
- Citation consistency score
- Local keyword rankings

### 5. Content Strategy
- Content gaps identified
- Page refresh priorities
- New content recommendations

### 6. Competitive Insights
- Where you stand vs. competitors
- Exploitable opportunities
- Threats to address

---

## Priority Matrix

| Priority | Impact | Effort | Examples |
|----------|--------|--------|---------|
| **P0 — Critical** | High | Low | Broken pages, HTTPS missing, mobile disasters |
| **P1 — High** | High | Medium | Thin content, missing title tags, no schema |
| **P2 — Medium** | Medium | Medium | Image optimization, internal linking gaps |
| **P3 — Low** | Low | High | Full content rewrites, new pillar pages |

---

## Common Issues by Website Type

### Photography / Creative Sites
- **Image bloat** → Compress all images to WebP, < 200KB
- **Portfolio thin text** → Add descriptive text to portfolio pages
- **Missing alt text** → Audit with Screaming Frog, add to all images
- **No service area pages** → Create location-specific landing pages
- **Slow LCP** → Lazy load images below fold, use CDN

### E-commerce
- **Duplicate product descriptions** → Rewrite with unique content
- **Faceted navigation crawl bloat** → noindex filter pages
- **Missing product schema** → Add Product JSON-LD
- **Thin category pages** → Add unique category descriptions

### Service Businesses
- **No location pages** → Create city/neighborhood landing pages
- **Weak service descriptions** → Expand with unique value props
- **No FAQ content** → Add FAQ schema with common questions
- **Missing CTAs** → Add to every service page

### Blogs / Content Sites
- **Thin content** → Expand to 1,000+ words for pillar posts
- **Keyword cannibalization** → Consolidate competing pages
- **Poor internal linking** → Add contextual links in body copy
- **Old content** → Update statistics, add new sections

---

## Reference Files

This skill references these detailed checklists:
- `references/technical-seo-checklist.md` — Full technical audit
- `references/local-seo-checklist.md` — Local SEO tasks
- `references/content-audit-template.md` — Content inventory template
- `references/competitor-analysis-template.md` — Competitive matrix

---

## Tools by Budget

| Budget | What to Use |
|--------|-------------|
| **Free** | Google Search Console, PageSpeed Insights, Screaming Frog (500 URLs), Ahrefs Webmaster Tools |
| **$50-100/mo** | Ubersuggest, Mangools (KWFinder), Serpstat |
| **$100-300/mo** | Ahrefs, Semrush, Moz Pro |
| **Enterprise** | BrightEdge, Conductor, Botify |
