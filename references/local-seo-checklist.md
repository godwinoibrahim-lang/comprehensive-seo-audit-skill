# Local SEO Checklist

Complete guide to optimizing for local search visibility.

## Google Business Profile (GBP) Optimization

### Setup & Verification
- [ ] Business claimed
- [ ] Verification completed (postcard, phone, or email)
- [ ] Primary category selected (most important)
- [ ] Secondary categories added (up to 9)

### Business Information
- [ ] Business name exact and consistent
- [ ] Address matches website and all citations
- [ ] Phone number local (not toll-free if local business)
- [ ] Website URL correct
- [ ] Service area defined (if service-based)
- [ ] Hours accurate and updated for holidays
- [ ] Appointment links added
- [ ] Description written (750 characters max, keyword-rich)

### Visual Content
- [ ] Logo uploaded
- [ ] Cover photo selected
- [ ] Interior photos (3-5)
- [ ] Exterior photos (2-3)
- [ ] Team/staff photos
- [ ] Product/service photos (5-10)
- [ ] Photos geotagged (optional but helpful)

### Posts & Updates
- [ ] Weekly posts scheduled
- [ ] Post types varied (updates, events, offers, products)
- [ ] Posts include images
- [ ] Posts include call-to-action
- [ ] COVID-19 update (if applicable)

### Q&A Section
- [ ] Questions pre-populated
- [ ] Answers helpful and keyword-rich
- [ ] FAQs match website content

### Reviews
- [ ] Review generation strategy
- [ ] All reviews responded to (positive and negative)
- [ ] Responses personalized
- [ ] Template system for efficiency

### Products/Services
- [ ] Services listed
- [ ] Products listed (if applicable)
- [ ] Pricing included where appropriate
- [ ] Descriptions keyword-rich

### Attributes
- [ ] Relevant attributes selected
- [ ] Accessibility info
- [ ] Amenities listed
- [ ] Health & safety (if applicable)

## NAP Consistency

### NAP = Name, Address, Phone

**Your NAP:**
- Name: 
- Address: 
- Phone: 
- Website: 

### Citation Audit

| Directory | URL | Name | Address | Phone | Status |
|-----------|-----|------|---------|-------|--------|
| Google Business Profile | | | | | |
| Bing Places | | | | | |
| Apple Maps | | | | | |
| Yelp | | | | | |
| Facebook | | | | | |
| Yellow Pages | | | | | |
| Industry-specific | | | | | |

### Top Citations to Build

**General:**
- Google Business Profile
- Bing Places
- Apple Maps
- Yelp
- Facebook
- Yellow Pages (YP.com)
- Better Business Bureau
- Chamber of Commerce
- Angie's List
- Thumbtack
- Nextdoor
- Foursquare

**Photography-Specific:**
- WeddingWire
- The Knot
- Here Comes The Guide
- Zola
- Fearless Photographers
- Junebug Weddings
- PPA (Professional Photographers of America)
- Local wedding/vendor directories

**Location-Specific:**
- Local business directories
- City/regional websites
- Local wedding directories
- Tourism bureaus
- Wedding venue vendor lists

## On-Site Local SEO

### Local Signals
- [ ] NAP on every page (footer or header)
- [ ] Embedded Google Map on contact/location pages
- [ ] Schema markup for LocalBusiness
- [ ] Location-specific landing pages
- [ ] Service area clearly defined

### Location Pages (if multiple)

**Each location page should have:**
- Unique URL (/locations/city-name/)
- Unique title and meta description
- Local phone number
- Specific address
- Embedded map
- Local testimonials
- Location-specific photos
- Nearby landmarks mentioned
- Local team members

### Content Localization

**Create content about:**
- [ ] Service areas/neighborhoods served
- [ ] Local venues (weddings, events)
- [ ] Local attractions/landmarks
- [ ] City/neighborhood guides
- [ ] Local client testimonials
- [ ] Local case studies
- [ ] Community involvement

**Content ideas for photographers:**
- "Best engagement photo locations in [city]"
- "Top wedding venues in [city] — photography guide"
- "What to expect from a [city] wedding photographer"
- "Seasonal photo opportunities in [city]"
- "[City] portrait photography locations"

## Local Link Building

### Local Link Opportunities

| Type | Examples | Priority |
|------|----------|----------|
| Local Directories | Chamber, city guides | High |
| Industry Directories | Wedding sites, photo orgs | High |
| Sponsorships | Local events, teams | Medium |
| Partnerships | Venues, vendors | High |
| Local Media | Newspapers, blogs | Medium |
| Community Involvement | Charities, events | Low |

### Local Link Tactics

1. **Venue Partnerships**
   - Get listed on vendor pages
   - Write guest posts for venue blogs
   - Offer styled shoots for venue portfolios

2. **Local Business Associations**
   - Chamber of Commerce
   - Wedding vendor associations
   - Business networking groups

3. **Sponsorships**
   - Local charity events
   - School sports teams
   - Community festivals

4. **Local PR**
   - Press releases for awards/achievements
   - Pitch local media stories
   - Offer expert commentary

5. **Guest Blogging**
   - Local lifestyle blogs
   - Wedding planning blogs
   - Regional publications

## Review Strategy

### Review Generation Tactics

**Automated:**
- Email follow-up after service
- SMS review requests
- Review cards in delivery package

**Manual:**
- Personal ask after great experience
- Vendor exchange (review for review)
- Contest/giveaway incentives

### Review Platforms (by priority)

1. Google (most important for local SEO)
2. Yelp
3. Facebook
4. WeddingWire/The Knot (for wedding photographers)
5. Industry-specific (Thumbtack, etc.)

### Review Response Templates

**Positive Review:**
```
Thank you [Name]! It was a pleasure working with you on [project]. [Personal detail]. We hope to see you again!
```

**Negative Review:**
```
We're sorry to hear about your experience, [Name]. This doesn't reflect our usual standards. [Brief explanation/remedy]. We'd love to make this right — please contact us at [email].
```

## Local Schema Markup

### LocalBusiness Schema

```json
{
  "@context": "https://schema.org",
  "@type": "PhotographyService",
  "name": "Godwin Oisi Studios",
  "image": "https://example.com/logo.jpg",
  "@id": "https://example.com",
  "url": "https://example.com",
  "telephone": "+1-123-456-7890",
  "priceRange": "$$$",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "123 Main St",
    "addressLocality": "Toronto",
    "addressRegion": "ON",
    "postalCode": "M5V 2K4",
    "addressCountry": "CA"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": 43.6532,
    "longitude": -79.3832
  },
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
      "opens": "09:00",
      "closes": "18:00"
    }
  ],
  "sameAs": [
    "https://facebook.com/yourpage",
    "https://instagram.com/yourpage"
  ]
}
```

### Service Area Schema (if applicable)

```json
{
  "@context": "https://schema.org",
  "@type": "PhotographyService",
  "name": "Godwin Oisi Studios",
  "areaServed": [
    {
      "@type": "City",
      "name": "Toronto"
    },
    {
      "@type": "City",
      "name": "Mississauga"
    },
    {
      "@type": "City",
      "name": "Vaughan"
    }
  ]
}
```

## Tracking Local SEO

### Key Metrics

| Metric | Tool | Target |
|--------|------|--------|
| Local Pack Rankings | BrightLocal/Local Falcon | Top 3 |
| GBP Insights Views | Google Business Profile | ↑ |
| GBP Insights Actions | Google Business Profile | ↑ |
| Direction Requests | GBP Insights | ↑ |
| Website Clicks from GBP | GBP Insights | ↑ |
| Phone Calls from GBP | GBP Insights | ↑ |
| Reviews Count | GBP | ↑ |
| Average Rating | GBP | 4.5+ |

### Google Business Profile Insights

**Track monthly:**
- How customers searched for you (direct vs. discovery)
- Where customers found you (Search vs. Maps)
- Customer actions (website visits, calls, direction requests)
- Photo views and photo quantity

### Local Rank Tracking

**Tools:**
- BrightLocal (best for local)
- Local Falcon (free grid tracker)
- Whitespark
- SEMrush Position Tracking

**Track for:**
- "photographer near me"
- "[service] in [city]"
- "[city] photographer"
- "best photographer [city]"

## Common Local SEO Issues

| Issue | Impact | Fix |
|-------|--------|-----|
| NAP inconsistent | Lost rankings | Audit and fix all citations |
| Wrong GBP category | Wrong traffic | Choose precise primary category |
| No location pages | Missed opportunities | Create service area pages |
| Fake/bad reviews | Reputation damage | Respond, report fake reviews |
| Duplicate GBP listings | Ranking confusion | Merge or remove duplicates |
| Service area unclear | Confused users | Define clearly in GBP and on site |
| No local content | Weak relevance | Create location-specific content |

## Photography-Specific Local SEO

### Venue Relationships
- Get on preferred vendor lists
- Submit real weddings to venue blogs
- Offer styled shoots for venue portfolios
- Tag venues in social posts

### Wedding Vendor Network
- Connect with planners, florists, venues
- Cross-promote on social media
- Referral partnerships
- Styled shoot collaborations

### Local Publications
- Submit real weddings to local blogs
- Pitch "best of" articles
- Offer photography tips to local media
- Sponsor local events

### Community Involvement
- Photograph charity events
- Donate sessions for auctions
- Volunteer photography skills
- Local business networking
