## Product & Technology Analysis: Criby (criby.com)

**Date:** 2026-05-25
**Analyst:** Product & Technology Research Agent
**Subject:** Criby -- "Planet Earth's Housing Department"

---

### Executive Summary

- **Criby is an early-stage global real estate marketplace built on Next.js (with Turbopack) and Mapbox, targeting buy/rent/list workflows across multiple countries.** The product is functional but clearly pre-scale: only ~12 listings are visible in the default view, and SimilarWeb reports just 647 total visits in April 2026 -- a dramatic contradiction to the claimed "1M+ monthly users."
- **The "70+ languages" claim relies entirely on ConveyThis, a third-party machine translation widget** that overlays automated translations on the UI. There is no evidence of human-translated content, localized listing data, or culturally adapted UX. The hreflang implementation covers ~15 languages via query parameters (e.g., `?locale=fr`), not dedicated language subdomains or paths.
- **The product has a thoughtful feature set for its stage** -- role-based onboarding (Seeker/Owner/Agent/Agency), verified agent badges, a Mapbox-powered map view with draw-to-search, rich listing detail pages with WhatsApp integration, and a tiered pricing model (Free/Pro/Enterprise). However, execution gaps are significant: no native mobile app, no sitemap.xml or robots.txt, no analytics integration detected, and sparse SEO infrastructure.
- **Trust and safety systems are surface-level.** "Verified" badges exist on agents and listings but no documentation explains the verification process. There is no visible escrow, no review/rating system for properties (only agent ratings), and the Terms of Service explicitly disclaim responsibility for disputes.
- **The product positions as global but operates primarily from/in Colombia (Medellin).** Google's SEO index title reads "#1 Medellin Real Estate," traffic is 100% from Colombia per SimilarWeb, and prices on the list view appear in USD but were previously reported in COP. The gap between global branding and local reality is the most critical product-market fit question.

---

### Detailed Findings

#### 1. Product Teardown

**Homepage & First Impression**
- Ultra-minimalist dark-themed landing page with a single centered CTA: "Search for a home" with a globe icon
- Tagline displayed: "PLANET EARTH'S HOUSING DEPARTMENT"
- Left sidebar navigation with icon-only links (no labels): Home, Menu/List, Filters, Messages, Map View, Grid View, and at bottom: Info, Profile, and another utility icon
- Theme color: `#1a1d2e` (deep navy-black)
- No hero images, no featured listings, no social proof on the homepage -- extremely sparse for a real estate marketplace

**Search & Discovery**
- **Search bar:** "Search city, neighborhood, address..." with autocomplete (appears to use geocoding)
- **Sort options:** Newest (default), with dropdown
- **Quick Filters:** Verified, Price Drop, Open House, Video Tour
- **Property Type filters:** Apartment, Penthouse, House, Commercial, Land, Business
- **Price slider:** $0 - $10.0M range
- **Size slider:** 0 m2 - 1.0K m2 (metric-only, no sq ft toggle despite sq ft displayed on cards)
- **Beds/Baths:** All, 1, 2, 3, 4+ selectors
- **Feature filters:** Pet Friendly, Balcony, Garden, Garage, Pool, Gym, Elevator, Security, Furnished, A/C, View, New Build
- **Saved Search & Alerts:** "Save Search" and "Get Alerts" buttons at bottom of filter panel
- **Draw-to-search:** Map view includes a "Draw" tool for polygon-based area search

**Map View (/map)**
- Full-screen Mapbox GL JS map in dark theme
- Defaults to user geolocation (tested: Long Beach, CA)
- Zoom controls (+/-) and compass/orientation button
- "0 homes" counter when no listings in view area
- No clustering indicators visible; listings may use point markers when present
- Map tiles load in ~5 seconds; no property pins visible in test area

**List View (/list)**
- Split-panel layout: map on left (~50%), listing cards on right
- Showed "12 Properties | 5 Boosted" in test
- Each listing card includes:
  - Property image with overlay badges (BUY/RENT, property type like "House"/"Apartment"/"LAND"/"BIZ", "NEW" indicator)
  - Title, address
  - Price (in USD) with per-sq-ft calculation
  - Beds, baths, sq ft
  - Agent name + avatar + "Verified Agent" badge
  - Time posted (e.g., "2h ago", "4h ago", "18h ago")
  - Action buttons: WhatsApp (green), Message, Save/Heart, Share
- No pagination controls visible -- likely infinite scroll

**Listing Detail Page (/property/{id})**
- URL structure: `/property/3` (numeric IDs, not slugs -- poor for SEO)
- **Photo gallery:** Multi-image grid layout with "Show all photos" button, "4+" indicator for overflow
- **Badges:** FOR SALE, House, VERIFIED (green dot)
- **Location tag:** "Forest Hills, Queens" with pin icon
- **Engagement metrics:** View count (e.g., "247"), time since posting ("3d ago")
- **Property specs:** Beds, bath, sq ft, $/sq ft
- **Description:** Text block with "read more" truncation
- **Amenities section:** Pill-style tags (Garden, Garage, Basement, Central AC, Hardwood Floors, Fireplace, Patio)
- **Report Spam:** Orange button visible on listing page (good trust signal)
- **Agent card (right sidebar):**
  - Agent photo, name, "Agent Verified" badge
  - "View All Properties" button
  - Stats: Response time (30 min), Rating (5 stars), Listings count (42)
  - Contact icons: Email, Message, WhatsApp, Share, Save/Heart
  - **"Schedule Meeting"** (purple CTA button)
  - **"Request a live tour"** (outlined button)
  - **"Get Notified When Live"** (teal/green CTA)
- **Map widget:** Mapbox embed showing property location with pin

**Onboarding / Signup (/signup)**
- Role-based account creation with 4 options:
  1. **Seeker** -- "I am looking to rent or buy a place"
  2. **Owner** -- "I own properties to rent or sell"
  3. **Agent** -- "I manage listings as an independent agent"
  4. **Agency** -- "I represent a brokerage or property team"
- Contextual note: "Agency teams can invite agents and assign listings after setup. Individual agents and owners can upgrade into team workflows later."
- Tagline on signup: "Choose how Criby should work for you. Pick the right path once, then Criby can shape onboarding, verification, dashboards, and property tools around your role."
- Sign in link for existing users
- No social login (Google, Facebook, Apple) observed at role-selection stage
- No visible phone verification or 2FA at this stage

**Messaging**
- Messages icon in left sidebar navigation
- Messages page (/messages) loads but requires authentication
- WhatsApp integration prominent on listing cards (green button) -- suggests off-platform messaging is primary
- In-platform messaging exists but couldn't be evaluated without account

**Mobile Experience**
- **No native iOS or Android app found** in App Store or Google Play searches
- **Responsive web:** When browser resized to 375x812 (iPhone dimensions), the layout DID NOT meaningfully adapt -- the left sidebar with icon navigation remained fixed, and content did not reflow. The mobile experience appears inadequate.
- The viewport meta tag is set (`width=device-width, initial-scale=1, viewport-fit=cover`) but the UI does not properly respond to narrow viewports
- No PWA manifest detected

#### 2. Localization & Language Infrastructure

**Translation Approach: ConveyThis Widget**
- The "70+ languages" claim is powered by **ConveyThis** (`cdn.conveythis.com/javascript/conveythis.js`)
- ConveyThis is a third-party SaaS translation overlay that provides machine translation via a JavaScript widget
- API key visible in page source: `pub_ba5e9ec995b6f82f10af183c52602864`
- This means: all translation is automated machine translation of the UI layer; no human review or localization is evident

**Hreflang Implementation**
The site implements hreflang alternate links for approximately 15 languages via query parameters:
- French (`?locale=fr`), German (`?locale=de`), Chinese (`?locale=zh`), Arabic (`?locale=ar`), Portuguese (`?locale=pt`), Russian (`?locale=ru`), Italian (`?locale=it`), Japanese (`?locale=ja`), Korean (`?locale=ko`), Farsi (`?locale=fa`), Spanish (`?locale=es`), Turkish (`?locale=tr`), and more
- Default language: English (`lang="en"`)
- URL pattern: Query parameter approach (`?locale=xx`) rather than subdirectories (`/fr/`) or subdomains (`fr.criby.com`) -- this is the weakest SEO pattern for multilingual sites

**Currency Implementation**
- Prices displayed in USD on the list view (when viewed from the US)
- WebFetch analysis previously showed prices in COP (Colombian Pesos) -- suggesting geolocation-based currency detection
- Price per square foot calculation shown alongside total price
- No visible currency toggle or selector for users to manually switch

**Unit Conversion**
- Listing cards show "sq ft" (imperial) when viewed from the US
- The filter panel uses "m2" (metric) for the size slider
- This inconsistency (mixed units within same page) suggests incomplete localization logic
- No user-facing toggle to switch between metric and imperial

**Content Localization Gaps**
- Listing descriptions appear to be in English only (no translated property descriptions observed)
- Agent names and property titles are not translated
- Amenity tags (Garden, Garage, etc.) would be machine-translated by ConveyThis but not natively localized
- No country-specific legal information or rental process guides
- No localized city/neighborhood pages

#### 3. Trust & Safety Systems

**Listing Verification**
- "VERIFIED" green badge appears on some listings and agents
- "Agent Verified" text below agent names on detail pages
- No documentation found explaining what "verified" means -- criteria are opaque
- Terms of Service mention listings must be "accurate" but don't detail verification procedures
- Pricing page mentions "Standard verification" (Free plan) vs. "Premium verification badge" (Pro plan) -- suggesting verification is tied to payment tier, not independent validation

**Identity Verification**
- No visible KYC/identity verification process in signup flow
- Agent directory page (/agents) shows filters for "Top Rated," "Most Listings," "Most Deals," "Most Experienced," "Fastest Response" -- but showed "0 agents found" in testing
- No government ID, license verification, or document upload visible in public-facing flows

**Fraud Prevention**
- "Report Spam" button visible on listing detail pages (orange, prominent)
- No visible phone verification for listing creators
- No duplicate listing detection or cross-reference system apparent
- Pricing page mentions "fee circumvention" prohibition in terms

**Payment & Escrow**
- Terms of Service reference "secure payment system" and separate "Payments Terms" (not found)
- No escrow service mentioned or visible
- Accepted payment methods (per pricing page): "major credit cards, PayPal, and bank transfers"
- No Stripe or payment processor scripts detected on public pages (likely gated behind auth)
- Commission structure: 10% on Free tier, 5% on Pro, custom on Enterprise
- Renter booking service fees: 5-10%

**Reviews & Ratings**
- Agent rating system visible (star rating on agent profile, e.g., "5 stars")
- No property/listing review system visible
- No Trustpilot or external review presence found for criby.com
- No user testimonials on the site

**Dispute Resolution**
- Terms explicitly state: Criby "bears no responsibility for disputes between parties or the condition of properties"
- Platform positions as marketplace intermediary only
- No visible dispute resolution mechanism, mediation service, or escalation path

#### 4. Technology Stack Analysis

**Confirmed Technologies**
| Component | Technology | Evidence |
|-----------|-----------|----------|
| Frontend Framework | **Next.js** (App Router with Turbopack) | `_next/static/chunks/turbopack-*` in script URLs, `__next` root element |
| Language/Runtime | **React** | Implied by Next.js; `__next` element present |
| Map Engine | **Mapbox GL JS** | Mapbox logo visible, dark-themed vector tiles |
| Translation | **ConveyThis** | External script `cdn.conveythis.com/javascript/conveythis.js` |
| CSS | **CSS Modules** (likely) + possibly **Tailwind CSS** | Class patterns suggest CSS Modules; no Tailwind CDN detected but class patterns partially match |
| Image Optimization | **Next.js Image Component** | `/_next/image` paths in page source |
| Protocol | **HTTP/2** | `nextHopProtocol: "h2"` in performance API |
| Hosting/CDN | **Vercel** (probable) | Next.js + Turbopack combination, `.vercel` patterns not confirmed but highly likely given stack |
| Icons | **SVG System** | 23 SVG resources loaded |
| Fonts | **Custom TTF fonts** | 3 TTF font files loaded |

**Not Detected / Absent**
- No Google Analytics, Google Tag Manager, or any analytics platform detected
- No Facebook Pixel, Hotjar, or user behavior tracking
- No Stripe.js or other payment SDK on public pages
- No Google Maps integration (uses Mapbox exclusively)
- No Leaflet or OpenStreetMap
- No service worker / PWA manifest
- No sitemap.xml (404)
- No robots.txt (404)
- No structured data / JSON-LD (empty array)
- No Open Graph tags
- No Twitter Card tags
- No canonical URL tag

**Performance Metrics (Homepage)**
| Metric | Value | Assessment |
|--------|-------|------------|
| DNS Lookup | 0ms | Excellent (cached) |
| TTFB | 51ms | Excellent |
| DOM Interactive | 306ms | Very Good |
| DOM Content Loaded | 306ms | Very Good |
| Full Page Load | 466ms | Excellent |
| Document Transfer Size | 5.9 KB | Very Small |
| Total Resources | 62 | Moderate |
| Total Transfer Size | 8.0 KB | Very Small (aggressive code splitting) |

The performance numbers are excellent, likely due to the minimal homepage having almost no content. This would likely degrade significantly on the map/list views with Mapbox and listing data loaded.

**SEO Infrastructure**
- **Critical gaps:** No sitemap.xml, no robots.txt, no structured data (JSON-LD/Schema.org), no Open Graph meta tags, no Twitter Cards, no canonical URL
- **Meta description:** "Global real estate platform - Buy, Sell, Rent properties worldwide" (generic, not keyword-optimized)
- **Title tag:** "Criby - Planet Earth's Housing Department" (branded, not descriptive)
- **Google indexed title:** "Criby | #1 Medellin Real Estate for Buying, Renting & Listing" (different from actual page title -- likely set via Google Search Console or Google's own rewrite)
- **URL structure:** `/property/3` (numeric IDs, no slugs, no location in URL -- poor for SEO)
- **Hreflang:** Present but uses query parameter pattern (`?locale=fr`) rather than subdirectories
- **SimilarWeb organic keywords:** 1 keyword total
- **Google site: search results:** Only 1 page indexed

**API Availability**
- Enterprise plan mentions "API access" and "Custom integrations"
- No public API documentation found
- No visible API endpoints in network requests from public pages
- ConveyThis makes API calls to `conveythis.com/languages/get` and `conveythis.com/website/code/get`

#### 5. Product Gaps & Opportunities

**Missing vs. Major Competitors**

| Feature | Criby Status | Zillow/Redfin | Properstar | Tranio |
|---------|-------------|---------------|------------|--------|
| Virtual Tours / 3D Walkthroughs | "Request a live tour" button exists; no self-serve 3D tours (Matterport/similar) | Yes (Matterport integration) | Limited | Some listings |
| AI Property Recommendations | None visible | Zestimate + recommendations | Basic matching | Manual curation |
| Neighborhood Insights / City Guides | None | Walk Score, school ratings, crime data | Market data | Country guides + legal info |
| Mortgage/Finance Calculator | None | Yes (integrated) | Partner referrals | Investment calculators |
| Saved Searches with Alerts | Present (Save Search + Get Alerts buttons) | Yes | Yes | Yes |
| Video Tours | Filter option exists ("Video Tour") but no listings found with this feature | Yes | Limited | Limited |
| Floor Plans | Not visible | Common | Some | Some |
| Price History / Zestimate | Not visible | Yes | Limited | Market trends |
| School/Transit/POI Data | Not visible | Yes | Limited | Country-level |
| Digital Lease / Contract Signing | Not visible; no mention in features | Emerging | No | No |
| Relocation Services | Not visible | No | Some | Yes (visas, legal) |
| Agent CRM / Pipeline | Mentioned in Pro plan ("Lead management tools") | Via partnerships | Via ListGlobally | Internal tools |
| Escrow / Secure Payments | Not visible | Via partnerships | No | Partial |
| User Reviews (Property-level) | Not visible | Yes | Limited | Limited |
| Native Mobile App | No (responsive web only, poorly adapted) | Yes (iOS + Android) | Yes (iOS + Android) | Yes |
| Blog / Content Marketing | /blog returns 404 | Extensive | Moderate | Extensive (country guides) |

**Critical Missing Features**
1. **No analytics/tracking at all** -- cannot measure user behavior, conversion funnels, or optimize
2. **No SEO foundation** -- no sitemap, no structured data, no robots.txt, 1 keyword indexed
3. **No content marketing** -- blog returns 404, no city guides, no market insights
4. **No native mobile app** -- and responsive web is poorly implemented
5. **No user reviews for properties** -- only agent ratings exist
6. **No neighborhood/area data** -- Walk Score, schools, transit, safety data all absent
7. **No mortgage/financing tools** -- critical for buy-side conversion
8. **No virtual tour hosting** -- only "request a live tour" which depends on agent availability

**Notable Features Present (for stage)**
1. Role-based onboarding (4 paths) with promise of adapted dashboards
2. WhatsApp integration on every listing card
3. Agent directory with performance metrics (response time, rating, listing count)
4. Draw-to-search on map
5. "Boosted" listings concept (monetization lever)
6. "Get Notified When Live" -- suggests upcoming live tour/streaming feature
7. Tiered pricing with free tier for listing (smart for supply-side growth)
8. Enterprise tier with white-label and API access

#### 6. Product Roadmap Speculation

**Based on Current Feature Signals**
1. **Live Video Tours** -- The "Request a live tour" and "Get Notified When Live" buttons strongly suggest real-time video tour functionality is in development or already gated behind authentication. The "Live" status indicator on some listings reinforces this.
2. **Video Tour Hosting** -- The "Video Tour" quick filter exists but no content matches it yet, suggesting this feature is being built.
3. **Agency Team Management** -- The Agency signup path mentions "invite agents and assign listings" -- a CRM/team management dashboard is either built or in progress.
4. **Lead Management** -- Listed as a Pro plan feature, suggesting pipeline/CRM tools for agents.
5. **White-Label Solution** -- Enterprise plan mentions "white-label options" and "custom branding" -- potentially pivoting to B2B infrastructure for real estate agencies.

**What They Should Build Next (Priority Order)**
1. **SEO Foundation** (critical) -- sitemap.xml, robots.txt, structured data, keyword-rich URLs, city landing pages. Currently invisible to search engines.
2. **Analytics Integration** (critical) -- Google Analytics or Mixpanel; they currently have zero visibility into user behavior.
3. **Mobile-Responsive Overhaul** (critical) -- The current responsive experience is broken; sidebar doesn't collapse on mobile.
4. **Content Engine** -- Blog, city guides, market reports, relocation guides. Essential for organic traffic.
5. **Matterport/3D Tour Integration** -- Self-serve virtual tour embeds would differentiate vs. local competitors.
6. **AI-Powered Recommendations** -- Property matching based on user preferences and behavior.
7. **Neighborhood Data Layer** -- Integrate Walk Score, school data, transit, safety overlays on the Mapbox map.
8. **Native Mobile App** -- PWA at minimum; native iOS/Android ideally.
9. **Escrow/Payment Integration** -- Stripe Connect or similar for secure cross-border transactions.
10. **Human Translation for Key Markets** -- Replace ConveyThis machine translation for top 5 languages with professional translation.

---

### Key Data Points

1. **SimilarWeb traffic (April 2026): 647 total visits** -- contradicts claimed "1M+ monthly users" by ~1,500x
2. **Traffic source: 100% Colombia** -- contradicts "100+ countries" global positioning
3. **Google organic keywords: 1** -- effectively zero SEO presence
4. **Google indexed pages: 1** (via site: search) -- severe crawlability issues
5. **Listings visible: 12** in default view, claimed "50K+ properties"
6. **Translation method: ConveyThis machine translation widget** -- not native localization
7. **Hreflang languages: ~15** (vs. claimed "70+ languages")
8. **Page load speed: 466ms full load, 51ms TTFB** -- excellent (but homepage is near-empty)
9. **Tech stack: Next.js + Turbopack + Mapbox GL JS + ConveyThis** -- modern but minimal
10. **Pricing: Free (3 listings), Pro ($47/mo approx at COP 193,550), Enterprise ($190/mo approx at COP 786,050)**
11. **Commission structure: 10% (Free), 5% (Pro), custom (Enterprise)**
12. **Agent directory: "0 agents found"** in live testing
13. **No native mobile app** exists; responsive web is poorly implemented
14. **No analytics platform** detected (no GA, GTM, Hotjar, Mixpanel, or similar)
15. **No sitemap.xml, no robots.txt** -- fundamental SEO infrastructure missing
16. **Signup roles: 4** (Seeker, Owner, Agent, Agency) -- thoughtful segmentation
17. **Founding year: 2024** -- less than 2 years old
18. **Listed team: CEO Sarah Chen, CTO Marcus Rodriguez, Head of Product Elena Kowalski, Head of Ops David Park** (from /about page; unable to verify via LinkedIn/Crunchbase)
19. **Contact: hi@criby.com, +1-440-MY-CRIBY (1-440-696-2749)** -- US phone number despite Colombia focus
20. **Protocol: HTTP/2** -- properly configured

---

### Strategic Implications

**The "Global vs. Local" Paradox**
Criby's most significant strategic tension is the gap between its global branding and its hyper-local reality. The platform brands itself as "Planet Earth's Housing Department" covering 100+ countries, but traffic data shows 100% Colombian users, Google indexes it as "#1 Medellin Real Estate," and the listing inventory appears to be concentrated in a handful of locations. The "50K+ properties" and "1M+ monthly users" claims appear to be aspirational or fabricated metrics, which creates a credibility risk if challenged.

**Technology is Modern but Incomplete**
The Next.js + Turbopack + Mapbox stack is solid and modern. The team clearly has frontend engineering capability. However, the absence of basic infrastructure (analytics, SEO, sitemap, structured data) suggests either a very small team, a focus on product features over growth infrastructure, or both. The ConveyThis translation approach is a pragmatic shortcut but won't scale for a serious international platform.

**Monetization Model is Well-Designed**
The tiered pricing (Free/Pro/Enterprise) with differentiated commission rates (10%/5%/custom) and feature gating (analytics, virtual tours, lead management at Pro+) is a smart marketplace model. The "Boosted" listings concept provides an additional revenue stream. However, with ~12 visible listings and 647 monthly visits, revenue is likely negligible.

**Competitive Position**
Criby is attempting to compete in a market with entrenched players at every level: Zillow/Redfin domestically, Properstar/Tranio/Idealista internationally, and dozens of local Medellin-specific agencies. Their differentiation claim is unclear. They lack the data moats (Zestimate, MLS access), content depth (city guides, market reports), user base, and brand recognition of established players. The "live tour" feature, if executed well, could be a meaningful differentiator for international buyers.

**Key Risks**
1. Inflated metrics undermine credibility with sophisticated partners/investors
2. No SEO strategy means zero organic discovery pipeline
3. No analytics means they cannot iterate on product-market fit
4. ConveyThis machine translation will produce poor quality for real estate content (legal terms, property descriptions)
5. The "verified" system without transparent criteria could become a trust liability
6. No escrow/payment protection exposes users to fraud risk in cross-border transactions

---

### Confidence Level

| Aspect | Confidence | Notes |
|--------|------------|-------|
| Tech stack identification | **High** | Directly verified via page source, JS inspection, and visual confirmation |
| Feature inventory | **High** | Observed directly via browser navigation and screenshot analysis |
| Traffic/usage claims debunking | **High** | SimilarWeb data directly contradicts claimed metrics |
| Translation approach | **High** | ConveyThis script and API key directly identified in page source |
| Pricing/monetization | **Medium-High** | Observed on pricing page; COP pricing may vary |
| Team/founding claims | **Low** | Listed on /about page but no external verification possible via LinkedIn/Crunchbase |
| Competitive positioning | **Medium** | Based on feature comparison; actual user preference data unavailable |
| Roadmap speculation | **Medium** | Based on UI signals and feature hints; no public roadmap or blog found |

---

### Sources & Methodology

**Primary Sources (Direct Observation)**
- criby.com -- Homepage, /map, /list, /property/3, /signup, /about, /pricing, /agents, /terms, /privacy (visited and analyzed May 2026)
- Browser JavaScript console -- Tech stack extraction via DOM inspection
- Chrome DevTools / Performance API -- Page load metrics

**Secondary Sources (Web Research)**
- [SimilarWeb -- criby.com traffic analysis](https://www.similarweb.com/website/criby.com/) -- 647 visits, 100% Colombia
- [Criby.com](https://criby.com/) -- Official website
- [ConveyThis](https://www.conveythis.com/) -- Translation widget provider documentation
- [Mapbox](https://www.mapbox.com/) -- Map technology provider
- [Google search: site:criby.com](https://www.google.com/search?q=site:criby.com) -- 1 indexed page
- [Tracxn -- Crib company profile](https://tracxn.com/d/companies/crib/__Gn3Dsnzquw50dRc2oyJM0w-ZfuLR8Fle-slbm6o5F9o) -- Different company (Crib India), not Criby
- [HomesGoFast -- International Property Portals](https://homesgofast.com/buy-property-abroad/the-75-best-international-property-portals/) -- Competitor landscape
- [EstateSkyline -- Top Property Listing Websites 2026](https://estateskyline.co/blog/top-property-listing-websites/) -- Market context

**Methodology**
1. Web search across multiple queries for company information, tech stack, reviews, team, funding
2. Direct website visit and screenshot analysis via Chrome browser automation
3. JavaScript-based technology detection (meta tags, scripts, frameworks, analytics, external services)
4. Performance API analysis for page load metrics
5. SimilarWeb traffic analysis for usage validation
6. Mobile responsiveness testing via browser resize to 375x812
7. Sitemap/robots.txt checks (both returned 404)
8. Signup flow and filter panel visual inspection
9. Cross-referencing claimed metrics against observable data

**Tools Used:** Chrome browser (direct inspection), WebSearch, WebFetch (page content analysis), SimilarWeb (traffic data), JavaScript DOM analysis, Performance API
