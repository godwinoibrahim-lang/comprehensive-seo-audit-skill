# Content Audit Template

Spreadsheet structure for conducting a comprehensive content audit.

## Spreadsheet Columns

| Column | Description | Data Type |
|--------|-------------|-----------|
| **URL** | Full page URL | Text |
| **Page Title** | Current <title> tag | Text |
| **Meta Description** | Current meta description | Text |
| **H1** | Current H1 heading | Text |
| **Word Count** | Body content word count | Number |
| **Content Type** | Page category | Dropdown |
| **Target Keyword** | Primary keyword | Text |
| **Current Ranking** | Avg position (GSC) | Number |
| **Organic Traffic** | Sessions (12 months) | Number |
| **Conversions** | Goal completions | Number |
| **Conversion Rate** | Conv rate % | Percent |
| **Bounce Rate** | % single page sessions | Percent |
| **Avg Time** | Time on page | Duration |
| **Last Updated** | Content freshness | Date |
| **Action** | Keep/Update/Remove/Merge | Dropdown |
| **Priority** | P0/P1/P2/P3 | Dropdown |
| **Notes** | Observations | Text |

## Content Type Categories

- Homepage
- Service Page
- Product Page
- About Page
- Blog Post
- Pillar Content
- Location Page
- Landing Page
- Portfolio/Gallery
- FAQ Page
- Contact Page
- Resource/Download
- Video/Audio
- Tool/Calculator

## Action Categories

### Keep
Page is performing well. Monitor for changes.

### Update
- [ ] Refresh outdated information
- [ ] Expand thin content
- [ ] Improve E-E-A-T signals
- [ ] Add/update images
- [ ] Optimize for target keywords
- [ ] Add internal links
- [ ] Improve CTAs

### Remove
- [ ] 301 redirect to relevant page
- [ ] Update internal links pointing to it
- [ ] Remove from navigation/sitemaps

### Merge
- [ ] Combine with similar content
- [ ] 301 redirect old URLs to new
- [ ] Consolidate link equity

### Consolidate
- [ ] Merge multiple thin pages
- [ ] Create comprehensive pillar page
- [ ] Redirect old URLs to new

## Scoring Matrix

### Traffic Score (0-10)
| Range | Score |
|-------|-------|
| 10,000+ visits | 10 |
| 5,000-9,999 | 8 |
| 1,000-4,999 | 6 |
| 500-999 | 4 |
| 100-499 | 2 |
| < 100 | 0 |

### Engagement Score (0-10)
Calculate: (Time on page factor + Low bounce rate factor) / 2

### Conversion Score (0-10)
| Conv Rate | Score |
|-----------|-------|
| > 5% | 10 |
| 3-5% | 8 |
| 2-3% | 6 |
| 1-2% | 4 |
| 0.5-1% | 2 |
| < 0.5% | 0 |

### Quality Score (0-10)
Manual assessment:
- Depth and comprehensiveness (0-3)
- E-E-A-T signals (0-3)
- User experience (0-2)
- Current optimization (0-2)

### Overall Content Score
(Traffic + Engagement + Conversion + Quality) / 4

## Audit Workflow

1. **Export data:**
   - All URLs from Screaming Frog
   - Traffic data from GA4
   - Ranking data from GSC or Ahrefs

2. **Merge in spreadsheet:**
   - Combine all data sources by URL
   - Use VLOOKUP or INDEX/MATCH

3. **Score each page:**
   - Automated scores for traffic/conversion
   - Manual scores for quality

4. **Assign actions:**
   - Top 20%: Keep
   - Middle 60%: Update
   - Bottom 20%: Remove/Merge

5. **Prioritize:**
   - High traffic + low score = Priority P0
   - Medium traffic + medium score = Priority P1
   - Low traffic + any score = Priority P2/P3

## Content Gap Analysis

### What to Look For

**Missing Topics:**
- What do competitors rank for that you don't?
- What questions do customers ask that aren't answered?
- What are trending topics in your industry?

**Content Depth:**
- Which pages are < 500 words?
- Which topics deserve comprehensive guides?
- Where can you add multimedia (video, infographics)?

**Content Formats:**
- Do you have how-to guides?
- Do you have case studies?
- Do you have comparison content?
- Do you have interactive tools?

### Competitive Content Analysis

For each competitor:
1. List their top-performing content
2. Identify content formats they use
3. Note content gaps you can fill
4. Identify unique angles they've missed

## Update Guidelines by Content Type

### Service Pages
- **Word count:** 500-1000 words
- **Structure:** Problem → Solution → Process → CTA
- **Updates needed:** Pricing, testimonials, process changes

### Product Pages
- **Word count:** 300-500 words + specs
- **Structure:** Benefits → Features → Specs → Reviews → CTA
- **Updates needed:** Availability, pricing, new reviews

### Blog Posts
- **Word count:** 1000-3000 words
- **Structure:** Hook → Context → Solution → Examples → CTA
- **Updates needed:** Annual refresh, new examples, updated stats

### Pillar Pages
- **Word count:** 3000-5000+ words
- **Structure:** Overview → Sections → Subtopics → Resources
- **Updates needed:** Quarterly review, new subtopic additions

## Content Refresh Checklist

When updating existing content:

- [ ] Update statistics and data
- [ ] Refresh examples and case studies
- [ ] Add new sections for subtopics
- [ ] Improve H2/H3 headings
- [ ] Add FAQ section
- [ ] Include new images/screenshots
- [ ] Add internal links to new content
- [ ] Update publish/refresh date
- [ ] Check for broken links
- [ ] Optimize for new keyword opportunities
- [ ] Add/update schema markup
- [ ] Share/promote refreshed content

## Content Calendar Template

| Month | Week | Content Piece | Type | Target Keyword | Status |
|-------|------|---------------|------|----------------|--------|
| Jan | 1 | Ultimate Guide | Pillar | guide to... | Planned |
| Jan | 2 | Case Study | Post | how [client]... | Planned |
| Jan | 3 | Video Tutorial | Video | how to... | Planned |
| Jan | 4 | Comparison | Post | vs... | Planned |

## Quick Win Opportunities

Look for:
1. Pages ranking positions 8-15 (page 2 of Google) — small boost gets page 1
2. Pages with high impressions but low CTR — title/meta optimization
3. Pages with high traffic but low conversion — CTA optimization
4. Pages with quick answers but no featured snippet — structured formatting
