# SEO Audit Skill — GitHub Repository

> A comprehensive, generic SEO audit skill for AI agents. Conduct full technical SEO audits, on-page analysis, local SEO checks, competitor research, and actionable improvement plans. Built for photographers, creatives, consultants, and small businesses — adaptable to any website type.

---

## 📋 What Is This?

A downloadable AI agent skill that systematizes SEO audits into a repeatable, thorough process. The skill guides a full SEO engagement from discovery to final recommendations — no expertise required beyond running the tool.

### What You Get

| File | Purpose |
|------|---------|
| `README.md` | This file — overview, quick start, contents |
| `SKILL.md` | **The main downloadable skill** — paste into any agent's skills directory |
| `USE_CASES.md` | 6 real-world examples across photography, e-commerce, service businesses |
| `references/` | Reference checklists (technical, on-page, local, competitive) |

---

## 🎯 Who This Is For

- **AI agents** that need a systematic SEO audit framework
- **Photographers / creatives** auditing their own sites
- ** consultants** doing SEO for clients
- **Small businesses** without dedicated SEO teams
- **Marketing generalists** who need to run an audit without prior SEO experience

---

## 🚀 Quick Start

### 1. Download the Skill

Copy `SKILL.md` to your agent's skills directory. For OpenClaw:

```bash
cp SKILL.md ~/.openclaw/skills/seo-audit/SKILL.md
```

### 2. Install References (Optional)

The skill references checklist files. Copy the `references/` folder alongside `SKILL.md`:

```bash
cp -r references/ ~/.openclaw/skills/seo-audit/references/
```

### 3. Run an Audit

Tell your agent:

> "Use the SEO Audit skill to audit [website URL]. Focus on: [technical / on-page / local / all]. Give me an overall health score, top 3 priorities, and quick wins."

---

## 📁 Repository Structure

```
seo-audit-skill/
├── README.md           ← This file
├── SKILL.md           ← The generic downloadable skill
├── USE_CASES.md       ← 6 real-world examples
└── references/
    ├── technical-seo-checklist.md
    ├── local-seo-checklist.md
    ├── content-audit-template.md
    └── competitor-analysis-template.md
```

---

## 🔍 What the Skill Covers

### Technical SEO
- Crawlability & robots.txt
- Indexing & canonical tags
- Site architecture & internal linking depth
- Core Web Vitals (LCP, FID/INP, CLS)
- HTTPS & security
- Mobile optimization

### On-Page SEO
- Title tags & meta descriptions
- Heading structure (H1, H2, H3)
- Content quality & word counts
- Image optimization & alt text
- Schema markup (JSON-LD)
- URL structure

### Local SEO
- Google Business Profile optimization
- NAP consistency across directories
- Local citations
- Embedded Google Maps
- Location-specific content

### Content Audit
- Content inventory & performance
- E-E-A-T assessment (Expertise, Experience, Authoritativeness, Trustworthiness)
- Content gap analysis
- Thin content identification

### Backlink Audit
- Referring domain profile
- Toxic link identification
- Anchor text distribution
- Lost/broken link reclamation

### Competitor Analysis
- Keyword gap analysis
- Content format benchmarking
- Backlink source replication
- Competitive positioning matrix

---

## 📊 Audit Output

The skill produces a structured report:

1. **Executive Summary** — Health score (0-100), top 3 priorities, quick wins
2. **Technical SEO Report** — All issues with severity and fix effort
3. **On-Page SEO Report** — Page-by-page optimization issues
4. **Local SEO Report** — GBP status, citations, local signals
5. **Content Strategy** — Gap analysis, refresh priorities, content calendar
6. **Competitive Insights** — Where you stand vs. competitors, opportunities

---

## 💡 Common Issues by Website Type

The skill includes specialized checklists for:

| Website Type | Typical Issues |
|--------------|----------------|
| Photography / Creative | Image bloat (slow speed), thin portfolio text, missing alt text, no service area pages |
| E-commerce | Duplicate product descriptions, faceted navigation crawl bloat, missing product schema |
| Service Businesses | No location pages, weak service descriptions, no FAQ content |
| Blogs / Content | Thin affiliate content, keyword cannibalization, poor internal linking |

---

## 🛠️ Tools the Skill Uses

| Budget | Tools |
|--------|-------|
| Free | Google Search Console, PageSpeed Insights, Screaming Frog (500 URL limit), Ahrefs Webmaster Tools |
| $50-100/mo | Ubersuggest, Mangools, Serpstat |
| $100-300/mo | Ahrefs, Semrush, Moz Pro |
| Enterprise | BrightEdge, Conductor, Botify |

---

## 📦 Contents

| File | Description |
|------|-------------|
| `README.md` | This overview file |
| `SKILL.md` | **The downloadable AI agent skill** — comprehensive SEO audit framework |
| `USE_CASES.md` | 6 real-world examples: photography site, e-commerce, local service, blog, migration, competitor analysis |
| `references/technical-seo-checklist.md` | Detailed technical audit checklist |
| `references/local-seo-checklist.md` | Local SEO-specific tasks |
| `references/content-audit-template.md` | Content inventory spreadsheet template |
| `references/competitor-analysis-template.md` | Competitive benchmarking framework |

---

## 🤝 Contributing

Found an issue or want to add a use case? Open an issue or PR. Common extensions:

- **Industry-specific checklists** (restaurants, real estate, lawyers)
- **Additional reference templates** (keyword research spreadsheet, link building outreach tracker)
- **Platform-specific guides** (Wix, Squarespace, WordPress, Pixieset gotchas)

---

## 📄 License

MIT — use it, adapt it, improve it.
