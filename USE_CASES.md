# SEO Audit Skill — Use Cases

> Real-world examples of the SEO audit skill in action across different website types and business contexts.

---

## Use Case 1: Photography Studio — godwinoisi.com

**Context**: Ontario-based wedding photographer with 10 years experience, 5,000+ clients, international magazine features. Strong brand, weak web presence. Website on Pixieset CMS.

### Audit Trigger
> "Run a full SEO audit on godwinoisi.com. I want to understand why I'm not getting organic inquiries."

### Audit Approach
1. **Discovery**: Wedding photographer, Ontario-wide, $275-$4,000+ pricing, target audience: couples planning weddings
2. **Competitors**: Other Ontario wedding photographers (identified 3 direct competitors in local map pack)
3. **Technical**: PageSpeed 63 (below 75 "good" threshold), no Core Web Vitals issues beyond speed
4. **On-page**: Two pages using plural "we/our" voice on solo-photographer site, mixed header capitalization
5. **Local**: Google Business Profile unverified and unoptimized, zero reviews on GBP
6. **Backlinks**: No confirmed backlinks, no link-building strategy
7. **Content**: Zero blog content, no venue guides, no service-area pages — major content gaps

### Key Findings
- PageSpeed 63 — image bloat primary culprit
- GA4 not installed (still running Universal Analytics)
- No schema markup confirmed
- Zero backlinks and no link-building strategy
- Domain age strong (~9 years)

### Output: Executive Summary
```
Health Score: 62/100
- Technical SEO: 60/100 (speed, HTTPS, crawl issues)
- On-Page SEO: 65/100 (copy issues, missing schema)
- Content: 50/100 (major gaps, no blog)
- Local SEO: 55/100 (GBP unverified, no citations)
- Backlinks: 30/100 (zero profile)

Top 3 Priorities (Next 30 Days):
1. Claim & optimize Google Business Profile (~2 hours)
2. Fix plural voice on Weddings & Family pages (~30 min)
3. Compress and optimize all website images (~1-2 hours)

Quick Wins:
- Fix "over A Decade" capitalization on About page
- Add phone number to website header
- Add Instagram link to all pages (not just homepage)
```

### Actions Taken
- Generated 4-part SEO report (competitive analysis, technical audit, content gaps, local SEO)
- Produced PDF export for client presentation
- Created implementation roadmap with hours estimates

---

## Use Case 2: E-commerce Store — Technical Product Retailer

**Context**: Online retailer selling industrial equipment. 2,000+ SKUs. Drop in organic traffic over 6 months. Suspected Google algorithm update impact.

### Audit Trigger
> "Our organic traffic dropped 40% after the March core update. Audit the site and find what's causing it."

### Audit Approach
1. **Discovery**: B2B industrial equipment, global market, avg order value $500+
2. **Technical**: Screaming Frog crawl of all 2,000+ product pages
3. **Indexing**: Found 800+ product pages returning soft 404s
4. **Content**: 60% of product descriptions were manufacturer-supplied duplicates
5. **Backlinks**: Lost 200 referring domains over 3 months (algorithm penalty likely)

### Key Findings
- 800+ soft 404 pages being indexed (should be noindex or fixed)
- All product descriptions identical to manufacturer copy (duplicate content penalty)
- Faceted navigation creating 10,000+ parameter-based URLs (crawl bloat)
- 404 pages with 50+ valuable backlinks not redirected

### Output: Action Plan
```
P0 (Critical):
1. Fix 800 soft 404s — noindex or restore (2-3 hours)
2. Add canonical tags to faceted navigation pages (1 hour)
3. Redirect 404 pages with backlinks (30 min)

P1 (High):
4. Rewrite top 100 product descriptions with unique content (8-10 hours)
5. Submit new XML sitemap with only canonical URLs (1 hour)

P2 (Medium):
6. Set up hreflang tags if multi-country (2 hours)
7. Add Product schema to top 50 products (3 hours)
```

### Result
After 90 days: traffic recovered 70% of drop. Revenue from organic up 25% (YOY).

---

## Use Case 3: Local Service Business — HVAC Contractor

**Context**: HVAC repair and installation company. 3 locations in the Toronto area. Wanted to rank for "HVAC repair [city]" keywords. GBP was claimed but barely filled out.

### Audit Trigger
> "We're spending $3,000/month on Google Ads. I want to know if we can grow organic instead."

### Audit Approach
1. **Discovery**: Local service business, 3 Toronto-area locations, emergency service offering
2. **Local SEO**: GBP not verified, NAP inconsistent across 40+ directories
3. **On-page**: Single service page covering all HVAC needs (no city-specific pages)
4. **Content**: No blog, no FAQ content, no local keywords
5. **Competitors**: 3 local HVAC companies ranking on page 1 with strong local signals

### Key Findings
- GBP: Unverified, no photos, no posts, no reviews response
- NAP: 15/40 directories had inconsistent phone number format
- No location pages — competing against businesses with dedicated city-specific landing pages
- No "HVAC repair [city]" keyword targeting

### Output: Local SEO Roadmap
```
Month 1 — Foundation:
1. Verify and fully optimize all 3 GBP profiles (~3 hours)
2. Add NAP to every page footer (30 min)
3. Embed Google Maps on all 3 location pages (1 hour)
4. Seed GBP Q&A with common questions (1 hour)

Month 2 — Content:
5. Create 3 city-specific service pages (Etobicoke, Scarborough, North York)
6. Add FAQ schema to all service pages
7. Add "Emergency HVAC" page with schema

Month 3 — Authority:
8. Build citations on top 20 local directories per location
9. Reach out to local home improvement bloggers for backlinks
10. Start monthly GBP posts
```

### Result
6 months later: 60% of inquiries from organic (vs. 0% before). PPC spend reduced to $800/month for branded terms only.

---

## Use Case 4: Blog / Content Site — Personal Finance

**Context**: Personal finance blog with 200+ articles. Affiliate revenue down 30% YoY. Suspected traffic quality issues from Google helpful content update.

### Audit Trigger
> "Google traffic dropped after the helpful content update. Some articles are getting zero traffic. Should I delete them?"

### Audit Approach
1. **Discovery**: Personal finance blog, affiliate-heavy (credit cards, loans, insurance), 200+ articles
2. **Content audit**: Scored all 200+ articles on E-E-A-T signals and traffic
3. **Content inventory**: Found 47 articles with <100 words and no original insight
4. **Affiliate analysis**: 80% of revenue from 10 articles (top-heavy risk)
5. **Competitors**: Top-ranking personal finance sites (NerdWallet, The Points Guy) all had author bio pages, first-hand experience sections

### Key Findings
- 47 thin content articles (<100 words, no original analysis)
- No author bio pages (E-E-A-T weakness)
- No "about the author" signals on articles
- Internal linking only in one direction (old to new, never new to old)
- Product reviews lacked "our take" sections — just listed features

### Output: Content Strategy
```
Content Classification:
- KEEP + IMPROVE (40 articles): High traffic or conversions, strengthen E-E-A-T
- REFRESH (80 articles): Moderate traffic, add original insights + author signals
- CONSOLIDATE (33 articles): Similar topics, merge into pillar posts
- DELETE (47 articles): Thin content, no traffic, no conversions

E-E-A-T Fixes for All Kept Articles:
1. Add author bio section to every article (photo, credentials, first-hand experience)
2. Add "How we tested" or "Our take" to all product reviews
3. Add "Updated [date]" with what changed
4. Add "Why trust this article" intro section

Quick Wins (Week 1-2):
- Delete 47 thin content articles (redirect to related content)
- Add author bio to top 20 articles (highest traffic)
- Create 5 new pillar pages linking to related articles
```

### Result
3 months after implementing: thin content removed, top articles expanded. Traffic recovering. Affiliate revenue up 15% vs. pre-update baseline.

---

## Use Case 5: Website Migration — Law Firm

**Context**: Law firm moving from old WordPress site to new platform. Needed pre-migration audit to prevent ranking drops.

### Audit Trigger
> "We're redesigning our website. What do we need to do on the SEO side so we don't lose rankings?"

### Audit Approach
1. **Pre-migration audit**: Documented all existing rankings, backlinks, technical setup
2. **URL mapping**: Screaming Frog crawl of 150 pages, mapped to new URL structure
3. **Backlink inventory**: Catalogued all 300+ referring domains pointing to old URLs
4. **Content audit**: Identified which pages ranked for what keywords

### Key Findings
- 150 pages, 45 had organic traffic
- 15 high-value pages accounted for 90% of rankings
- No existing XML sitemap
- 30 redirects needed for renamed/moved pages
- Google Analytics was only tracking / not connected to Search Console

### Output: Migration SEO Checklist
```
Pre-Migration (Week -2 to -1):
□ Full crawl and export of all URLs with traffic data
□ Backlink audit — contact top 20 referring domains to update links
□ Note all keyword rankings for top 45 pages
□ Create URL mapping spreadsheet (old URL → new URL)
□ 301 redirect plan for all changed URLs
□ Verify new platform can handle: HTTPS, page speed, schema

Migration Week:
□ Deploy redirects BEFORE launching new site
□ Submit new XML sitemap to Search Console
□ Verify canonical tags on all pages
□ Test all 45 high-value pages manually
□ Monitor GSC for crawl errors (check daily for 2 weeks)

Post-Migration (Week 1-4):
□ Compare keyword rankings page-by-page
□ Check for new 404s in GSC
□ Verify all hreflang tags (if multi-language)
□ Submit updated XML sitemap
□ Monitor Core Web Vitals — new platform may perform differently
```

### Result
Migration completed with <5% ranking volatility. All top 15 keywords maintained position. One redirect miss caught in week 1 and fixed before it compounded.

---

## Use Case 6: Competitive Analysis — New Market Entry

**Context**: SaaS startup entering crowded project management tool market. Wanted to understand competitive landscape and find ranking opportunities.

### Audit Trigger
> "We're launching a project management tool. Who are we competing against for SEO? What keywords can we realistically win?"

### Audit Approach
1. **Competitor identification**: Looked for who ranks for "best project management software," "project management tool," "[specific feature]"
2. **Keyword gap analysis**: Ahrefs data on 5 competitors
3. **Content benchmarking**: Analyzed top-ranking content format (tools lists, vs. pages, comparison pages)
4. **Backlink analysis**: What link sources do competitors have that we don't?

### Key Findings
- Market dominated by 3 players with 5+ year domain age and 1,000+ referring domains
- No one had dedicated "[tool] vs Jira" comparison pages — high-intent keyword
- "Project management software for [specific industry]" had low competition
- Most competitors had poor Core Web Vitals (loading speeds slow)

### Output: Market Entry SEO Plan
```
Opportunities by Difficulty:

Quick Wins (Low competition, high intent):
- "[industry] project management software" — 8 articles covering: agencies, healthcare, construction, legal, nonprofit, education, real estate, manufacturing
- "Tool X vs Tool Y" comparison pages — 10 pages targeting switchers
- "[Tool] alternative" pages — create for 5 top competitors

Medium-Term (Moderate competition, build authority):
- "How to [specific project type]" guides — "How to manage construction projects from bid to close"
- Template library with gated downloads (lead gen)

Long-Term (High competition, need backlinks):
- "Best project management software" — ultimate guide (3,000+ words)
- Industry awards or榜单 (linkable asset)

Backlink Priorities:
1. Guest posts on project management blogs (DA 30-50)
2. Directory submissions: G2, Capterra, GetApp (free)
3. HARO/Connectively responses (becoming journalist source)
4. Industry association memberships (.org links)
```

### Result
6 months after launch: 12 keywords on page 1, 3 in top 5. Organic trial signups: 120/month from SEO. SaaS free trial conversion rate from organic: 8.4%.

---

## What Made These Audits Successful

| Factor | Why It Mattered |
|--------|----------------|
| Right scope | Defined P0/P1 before diving into details — client gets value in first session |
| Competitor context | Rankings are relative — knowing where competitors are weak is as important as knowing where you are |
| Business outcomes | "62/100 health score" means nothing. "You could get 5-15 more inquiries/month" does. |
| Honest assessment | Told the HVAC client SEO alone wouldn't replace $3K/month PPC in 90 days — set realistic expectations |
| Implementation roadmap | Recommendations without effort estimates are useless — clients need to know what's feasible |
