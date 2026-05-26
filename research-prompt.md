# Criby Deep Research — Multi-Agent Prompt System

**Target Company:** Criby (criby.com)
**Tagline:** "Planet Earth's Housing Department"
**What they do:** Global, multilingual real estate marketplace for buying/renting homes across 100+ countries. Founded 2024.
**Leadership:** Sarah Chen (CEO/Co-founder), Marcus Rodriguez (CTO/Co-founder), Elena Kowalski (Head of Product), David Park (Head of Operations)
**Claimed stats:** 50K+ properties, 100+ countries, 1M+ monthly users, 70+ languages

---

## MASTER ORCHESTRATION INSTRUCTIONS

Deploy the following 10 research agents in parallel. Each agent produces a self-contained research brief in a consistent format. Once all agents complete, deploy the Synthesis Agent to compile the final research paper.

**Output format for every sub-agent:**

```
## [Section Title]

### Executive Summary
(3-5 bullet points — the "so what" of this section)

### Detailed Findings
(Full research with data, analysis, and citations where possible)

### Key Data Points
(Numbered list of quantifiable facts, stats, and metrics)

### Strategic Implications
(What this means for the business — strengths, weaknesses, opportunities, threats)

### Confidence Level
(High / Medium / Low — based on data availability and source quality)

### Sources & Methodology
(Where the data came from, what was searched, any gaps)
```

---

## AGENT 1: Market & Industry Landscape

**Mission:** Map the entire global proptech and cross-border housing market that Criby operates in.

**Research the following:**

1. **Total Addressable Market (TAM)**
   - Global real estate market size (residential buy + rent)
   - Cross-border / international housing segment specifically
   - Online real estate marketplace revenue (global)
   - Break down by region: North America, Europe, LATAM, Asia-Pacific, Middle East/Africa

2. **Serviceable Addressable Market (SAM)**
   - International relocation market size (corporate + individual)
   - Expat population worldwide and growth trends
   - Digital nomad population estimates and projections
   - International student housing market
   - Cross-border rental transaction volume

3. **Serviceable Obtainable Market (SOM)**
   - Realistic capture rate for a new entrant in year 1-3
   - Comparable marketplace penetration benchmarks (what did Airbnb, Zillow, HousingAnywhere capture early on?)

4. **Industry Growth Drivers**
   - Remote work adoption and its impact on international living
   - Digital nomad visa programs (how many countries now offer them?)
   - Corporate relocation trends post-COVID
   - International student mobility trends
   - Retirement migration patterns
   - Investment property cross-border purchasing trends

5. **Industry Headwinds**
   - Housing regulation tightening globally (rent controls, short-term rental bans)
   - Economic slowdowns impacting mobility
   - Visa/immigration policy shifts
   - Currency volatility impact on cross-border transactions

6. **Market Maturity & Timing**
   - Where is this market in the adoption curve?
   - Is this a "why now" moment? What macro trends make 2024-2026 the right time?
   - Historical attempts at global housing platforms — what worked, what failed, why?

---

## AGENT 2: Competitive Landscape & Positioning

**Mission:** Identify every competitor — direct, indirect, and adjacent — and map Criby's positioning relative to them.

**Research the following:**

1. **Direct Competitors (Global/Cross-border housing platforms)**
   - HousingAnywhere
   - Spotahome
   - Nestpick (if still active)
   - Flatio
   - Uniplaces
   - Any other global rental/buy platforms
   - For each: founding year, funding raised, markets served, property count, revenue model, unique differentiators

2. **Regional Giants (Criby must displace or coexist with)**
   - Zillow / Redfin / Realtor.com (US)
   - Rightmove / Zoopla / OnTheMarket (UK)
   - Idealista / Fotocasa (Spain)
   - Immobilienscout24 / Immowelt (Germany)
   - Funda (Netherlands)
   - Domain / REA Group (Australia)
   - 99.co / PropertyGuru (Southeast Asia)
   - Lamudi (emerging markets)
   - OLX / Mercado Libre (LATAM classifieds with housing)
   - What is Criby's argument for why users would use them instead of the local platform?

3. **Adjacent Competitors**
   - Airbnb (long-term stays / monthly rentals pivot)
   - Booking.com (extended stays)
   - Facebook Marketplace (housing listings)
   - Furnished Finder
   - Nomad-focused platforms (NomadList, Remote Year)
   - Corporate relocation companies (BGRS, Cartus, SIRVA)

4. **Competitive Moat Analysis**
   - What defensible advantages could Criby build?
   - Network effects potential (two-sided marketplace dynamics)
   - Data moat possibilities
   - Brand / trust moat in a fraud-heavy space
   - Multi-language / localization as a barrier to entry

5. **Positioning Map**
   - Where does Criby sit on: Global vs. Local, Buy vs. Rent, Short-term vs. Long-term, Consumer vs. Corporate?
   - What is the white space they're targeting?
   - Is their positioning differentiated enough to win?

6. **Competitive Wedge Analysis**
   - What is the specific wedge Criby uses to enter the market?
   - Which customer segment do they win first? (likely: expats/digital nomads renting internationally)
   - How does the wedge expand into broader market capture?
   - Is the wedge defensible or easily copied?

---

## AGENT 3: Ideal Customer Profile (ICP) & Segmentation

**Mission:** Build a granular, data-backed picture of who Criby's customers are — both demand side (home seekers) and supply side (property listers/landlords).

**Research the following:**

1. **Demand Side — Primary Segments**

   **Segment A: Digital Nomads**
   - Population size and growth rate
   - Demographics (age, income, nationality distribution)
   - Housing preferences (furnished, short-to-mid-term, flexible)
   - Pain points with current solutions
   - Top destination cities
   - Spending patterns on housing
   - How they currently find housing (Facebook groups, Airbnb, word of mouth?)

   **Segment B: Corporate Relocators / Expats**
   - Annual global relocation volume
   - Average relocation budget
   - Decision-maker (individual vs. employer/relocation company)
   - Pain points (speed, verification, lease compliance, family needs)
   - Typical lease duration
   - Key corridors (US→Europe, Asia→US, etc.)

   **Segment C: International Students**
   - Annual international student flow (UNESCO data)
   - Top destination countries for students
   - Housing budget ranges
   - Pain points (scams, deposits from abroad, language barriers, guarantor requirements)
   - Current solutions used

   **Segment D: Retirees / Lifestyle Migrants**
   - Population moving abroad for retirement
   - Top retirement destinations
   - Buy vs. rent preference
   - Budget ranges
   - Decision timeline (research phase can be 1-2 years)

   **Segment E: Cross-border Property Investors**
   - Volume of international property investment
   - Top investment corridors
   - Motivations (yield, diversification, golden visas)
   - Information needs (ROI data, tax implications, management)

2. **Supply Side — Property Listers**

   **Who lists on a platform like this?**
   - Individual landlords with properties in popular expat/nomad destinations
   - Property management companies
   - Real estate developers with international buyer interest
   - Co-living operators (Selina, Outsite, etc.)
   - Corporate housing providers

   **Supply-side pain points:**
   - Reaching international tenants (language, trust, payment)
   - Vacancy in markets dependent on foreign demand
   - Currency and cross-border payment handling
   - Tenant verification across borders

3. **ICP Prioritization**
   - Which segment should Criby prioritize and why?
   - What's the sequencing strategy? (Win segment A first → expand to B → then C?)
   - LTV analysis by segment (who's worth most long-term?)
   - CAC analysis by segment (who's cheapest to acquire?)

---

## AGENT 4: Business Model & Monetization Deep Dive

**Mission:** Reverse-engineer how Criby makes (or will make) money and evaluate the economics.

**Research the following:**

1. **Revenue Model Analysis**
   - What revenue model do they appear to use? (Examine the platform for clues — paid listings, subscriptions, transaction fees, etc.)
   - Compare with how competitors monetize:
     - HousingAnywhere: service fee to tenants (typically ~1 month rent)
     - Spotahome: booking fee to tenants + landlord subscription
     - Zillow: premier agent advertising, Zillow Rentals fees
     - Airbnb: split service fee (guest + host)
   - What model makes most sense for Criby given their positioning?

2. **Potential Revenue Streams**
   - **Tenant/buyer service fees** — % or flat fee on transactions
   - **Landlord subscription tiers** — free listing + premium visibility
   - **Featured/promoted listings** — paid placement
   - **Lead generation** — selling qualified leads to agents/landlords
   - **Corporate relocation packages** — B2B pricing for companies
   - **Financial services** — rent insurance, deposit alternatives, currency exchange
   - **Data/analytics** — market intelligence for investors/developers
   - **Advertising** — moving companies, insurance, furniture, local services

3. **Unit Economics Modeling**
   - Average transaction value (monthly rent or purchase price)
   - Take rate assumptions (what % can they charge?)
   - Customer acquisition cost (CAC) estimates by channel
   - Lifetime value (LTV) estimates by segment
   - LTV:CAC ratio projections
   - Path to contribution margin positive

4. **Marketplace Economics**
   - Chicken-and-egg problem: how do they solve cold start?
   - Which side do they subsidize? (likely supply — get listings first)
   - Liquidity metrics that matter (matches per listing, time-to-fill)
   - Geographic density requirements (do they need critical mass city-by-city?)

5. **Pricing Strategy**
   - How should they price relative to competitors?
   - Free vs. freemium vs. paid — what tier structure?
   - Pricing psychology for international users (different willingness to pay by country)

6. **Revenue Projections**
   - Based on claimed 1M monthly users, what's implied revenue at various conversion/take rates?
   - Comparable marketplace revenue milestones (Airbnb at similar stage, HousingAnywhere, etc.)

---

## AGENT 5: Product & Technology Analysis

**Mission:** Tear down Criby's product, evaluate the tech, and identify strengths/gaps.

**Research the following:**

1. **Product Teardown**
   - Core features visible on the platform (search, filters, map view, list view, messaging)
   - Listing detail pages — what info is provided?
   - Search experience — how good is discovery? (filters for price, location, property type, amenities)
   - Onboarding flow for tenants/buyers
   - Onboarding flow for landlords/agents
   - Mobile experience (responsive web? native app?)

2. **Localization & Language Infrastructure**
   - How are 70+ languages handled? (machine translation, human translation, hybrid?)
   - Quality of translations (test a few languages)
   - Currency conversion — real-time rates? Built-in or third-party?
   - Unit conversion (sq ft vs. m2 — they have this)
   - Localized content vs. just translated UI

3. **Trust & Safety Systems**
   - How are listings verified? What claims do they make?
   - Identity verification for landlords/tenants
   - Fraud prevention measures
   - Secure payment/escrow systems
   - Review/rating system
   - Dispute resolution process

4. **Technology Stack Indicators**
   - What tech appears to power the site? (check page source, job listings for tech clues)
   - Performance (page load speed, responsiveness)
   - SEO infrastructure (meta tags, structured data, URL structure)
   - API availability for partners/integrations

5. **Product Gaps & Opportunities**
   - What features are missing compared to competitors?
   - Virtual tours / 3D walkthroughs?
   - AI-powered recommendations?
   - Neighborhood insights / city guides?
   - Integration with relocation services (visa, banking, insurance)?
   - Lease management / digital contracts?

6. **Product Roadmap Speculation**
   - Based on job postings, blog posts, or feature hints — where is the product heading?
   - What should they build next to drive retention and expand TAM?

---

## AGENT 6: Go-to-Market & Growth Strategy

**Mission:** Analyze how Criby acquires users and grows, and evaluate the effectiveness.

**Research the following:**

1. **Current Growth Channels (Evidence-Based)**
   - **SEO:** Check their domain authority, organic keyword rankings, content strategy
   - **Content Marketing:** Blog? Guides? City-specific content?
   - **Social Media:** Presence on Instagram, TikTok, LinkedIn, YouTube, Twitter/X — follower counts, engagement, content style
   - **Paid Acquisition:** Any evidence of Google Ads, Meta ads, display?
   - **Partnerships:** Any announced partnerships with relocation companies, universities, employers?
   - **PR/Media:** Press mentions, launch coverage, founder interviews
   - **Community:** Any forums, Discord, expat community engagement?
   - **Referral Program:** Do they have one?

2. **SEO Deep Dive**
   - Domain age and authority
   - Estimated organic traffic
   - Top ranking keywords
   - Content gap analysis vs. competitors
   - International SEO strategy (hreflang, country-specific pages)
   - City/neighborhood landing pages — do they exist?

3. **Growth Loops Analysis**
   - What organic growth loops could work? (Landlord lists → tenant finds → tenant becomes landlord later? Unlikely but explore)
   - SEO content loop (city guides → organic traffic → signups → listings)
   - Word-of-mouth / viral coefficient in expat communities
   - Supply-side growth: how do they get landlords in 100+ countries?

4. **Geographic Expansion Strategy**
   - Do they go wide (100 countries thin) or deep (10 countries thick)?
   - Evidence of which markets have most listings/activity
   - Localization requirements per market
   - Regulatory requirements per market

5. **Channel Strategy Recommendations**
   - What channels should they double down on?
   - What's the most efficient CAC channel for each ICP segment?
   - B2B channel for corporate relocation segment
   - Influencer/creator strategy (nomad influencers, expat YouTubers)

6. **Growth Benchmarks**
   - How do their claimed numbers (1M monthly users, 50K listings) compare to competitors at similar stage?
   - What growth rate would be "good" for a marketplace at this stage?
   - Time-to-liquidity benchmarks from other marketplace startups

---

## AGENT 7: Regulatory, Legal & Risk Analysis

**Mission:** Map every regulatory, legal, and operational risk Criby faces operating globally.

**Research the following:**

1. **Real Estate Licensing Requirements**
   - Which countries require a license to operate a real estate marketplace?
   - Brokerage vs. marketplace legal distinction by jurisdiction
   - Advertising regulations for property listings (truth in advertising, required disclosures)
   - How do competitors handle multi-jurisdiction compliance?

2. **Data Privacy & Protection**
   - GDPR compliance (European users)
   - CCPA (California users)
   - Data localization requirements by country
   - Cross-border data transfer restrictions
   - User data handling for identity verification

3. **Financial Regulations**
   - If handling payments/escrow — money transmitter licenses needed?
   - Anti-money laundering (AML) requirements for property transactions
   - Know Your Customer (KYC) obligations
   - Currency exchange regulations

4. **Consumer Protection**
   - Tenant rights variations by country
   - Deposit protection schemes (required in UK, Germany, etc.)
   - Cooling-off periods for property transactions
   - Disclosure requirements for landlords

5. **Platform Liability**
   - Liability for fraudulent listings
   - Liability for property condition misrepresentation
   - Terms of service enforceability across jurisdictions
   - Insurance requirements

6. **Operational Risks**
   - Fraud at scale (fake listings, identity fraud, payment fraud)
   - Marketplace trust collapse risk (one viral scam story can kill trust)
   - Supply quality control across 100+ countries
   - Currency risk on held funds
   - Geopolitical risk (operating in unstable markets)

7. **Tax Implications**
   - Tax nexus in multiple countries from operating there
   - VAT/GST on service fees
   - Withholding tax on cross-border payments
   - Tax reporting obligations (e.g., IRS reporting for US landlords)

---

## AGENT 8: Financial & Funding Analysis

**Mission:** Research Criby's financial position, funding history, and investment landscape.

**Research the following:**

1. **Funding History**
   - Any announced funding rounds? (Check Crunchbase, PitchBook, TechCrunch, press releases)
   - Investors — who backed them?
   - Valuation at last round
   - Total raised to date
   - If no public funding info — what does that imply? (bootstrapped, stealth, pre-seed?)

2. **Comparable Company Valuations**
   - What are proptech / housing marketplace companies valued at?
   - Revenue multiples in the space
   - Recent funding rounds in similar companies (2023-2025)
   - Recent exits / acquisitions in the space
   - Public company comps (Zillow, REA Group, Rightmove market caps and multiples)

3. **Investment Landscape**
   - Which VCs are active in proptech/marketplace investing?
   - Is proptech funding trending up or down?
   - What thesis would an investor need to believe to back Criby?
   - Key metrics investors look for in marketplace startups at this stage

4. **Burn Rate & Runway Estimates**
   - Based on team size and operational scope, estimated monthly burn
   - With claimed traction, how much runway do they likely have?
   - When would they need to raise next?

5. **Financial Benchmarks**
   - Marketplace gross merchandise volume (GMV) benchmarks
   - Revenue per listing benchmarks
   - Revenue per user benchmarks
   - Path to profitability comparisons

---

## AGENT 9: Team, Culture & Organizational Analysis

**Mission:** Research the founding team, hiring patterns, and organizational signals.

**Research the following:**

1. **Founder Deep Dive**
   - Sarah Chen (CEO) — background, previous companies, education, LinkedIn, public talks/interviews
   - Marcus Rodriguez (CTO) — technical background, previous engineering roles, open source contributions
   - Founder-market fit analysis — do they have relevant experience?
   - Have they worked together before?

2. **Leadership Team**
   - Elena Kowalski (Head of Product) — background
   - David Park (Head of Operations) — background
   - Any other notable hires?
   - Board members or advisors (if known)

3. **Hiring Signals**
   - Current job openings (check careers page, LinkedIn, AngelList/Wellfound)
   - What roles are they hiring for? (indicates priorities — engineering? sales? international expansion?)
   - Location of hires (HQ location, remote-first?)
   - Team size estimates from LinkedIn

4. **Culture Signals**
   - Glassdoor / employer review sites
   - Engineering blog or tech talks?
   - Conference presence
   - Open source contributions

5. **Advisory & Network**
   - Any notable advisors?
   - Accelerator/incubator participation?
   - Industry organization memberships

---

## AGENT 10: Strategic Assessment & The Wedge

**Mission:** Synthesize a strategic point of view on Criby's overall positioning, wedge, and path to winning.

**Research the following:**

1. **The Wedge — Deep Analysis**
   - What is the specific entry point Criby uses to crack the market?
   - Is the wedge "international renters who can't use local platforms due to language/trust barriers"?
   - How big is this wedge? Is it big enough to build a VC-scale business on?
   - Is the wedge expanding (more people relocating internationally) or contracting?
   - Can competitors easily replicate the wedge? (Can Zillow just add 70 languages?)
   - Does the wedge create a natural expansion path? (International renters → international buyers → all renters → all buyers?)

2. **Why Now?**
   - Remote work explosion post-COVID
   - Digital nomad visa proliferation (50+ countries now)
   - Gen Z/Millennial comfort with cross-border living
   - AI making real-time translation viable at scale
   - Increased international student mobility
   - What macro tailwinds are they riding?

3. **Why Them?**
   - What makes this team uniquely positioned?
   - First-mover advantage in truly global housing?
   - Technology advantage (localization infrastructure)?
   - Network advantage?

4. **Bull Case — Why Criby Wins**
   - Global housing is a $XX trillion market with no global platform
   - Airbnb proved global housing marketplace can work, but left long-term rentals underserved
   - Language/trust barriers create real friction that a purpose-built platform solves
   - Network effects compound — more listings in Barcelona attract more expats, which attract more landlords
   - Winner-take-most dynamics in marketplace businesses
   - Expansion from rental → buy → financial services → relocation services = massive TAM expansion

5. **Bear Case — Why Criby Struggles**
   - Real estate is inherently local — global aggregation has limited value
   - Local platforms have deep moats (regulatory knowledge, listing inventory, brand trust)
   - Chicken-and-egg problem is brutal across 100+ countries simultaneously
   - Verification at global scale is extremely hard and expensive
   - Low transaction frequency (people move 1-2x per decade) limits LTV
   - Regulatory complexity across 100+ jurisdictions is a nightmare
   - 1M monthly users claim seems aggressive for a 2024 startup — is it real?

6. **Strategic Recommendations**
   - If you were advising Criby, what would you tell them?
   - Focus strategy: go deep in 5-10 key corridors vs. thin global coverage?
   - Monetization priority: which revenue stream to prove first?
   - Partnership strategy: white-label for corporate relocation companies?
   - Expansion sequencing: which markets to prioritize?

7. **Key Questions to Answer**
   - Is the "global housing platform" a real category or a fantasy?
   - Can one platform truly serve NYC and Nairobi equally well?
   - Is verification at global scale technically and economically feasible?
   - What's the minimum viable liquidity per city to provide a good user experience?
   - How do you acquire supply in 100+ countries without an army of local teams?

---

## SYNTHESIS AGENT — Final Research Paper

**Mission:** Take the outputs from all 10 research agents and compile a comprehensive, executive-grade research paper.

**Paper Structure:**

### 1. Executive Summary (1 page)
- Company overview
- Market opportunity assessment (with numbers)
- Competitive positioning verdict
- Strategic assessment (bull/bear/base case)
- Overall rating: Strong / Promising / Risky / Weak

### 2. Company Overview
- What Criby does
- Founding story and team
- Current traction and stage
- Funding status

### 3. Market Opportunity
- TAM/SAM/SOM analysis with sources
- Growth drivers and headwinds
- Timing assessment ("why now")
- Market maturity and adoption curve position

### 4. Customer Analysis
- ICP breakdown with sizing per segment
- Demand-side pain points and alternatives
- Supply-side dynamics
- Segment prioritization recommendation

### 5. Competitive Landscape
- Direct, regional, and adjacent competitor mapping
- Positioning analysis and white space identification
- Competitive moat assessment
- Feature comparison matrix

### 6. Business Model & Economics
- Revenue model analysis
- Unit economics estimates
- Marketplace dynamics assessment
- Financial projections / scenario modeling

### 7. Product & Technology
- Product teardown findings
- Localization infrastructure assessment
- Trust & safety evaluation
- Product gap analysis

### 8. Go-to-Market & Growth
- Current growth strategy evaluation
- Channel effectiveness assessment
- Geographic expansion analysis
- Growth benchmarks vs. peers

### 9. Regulatory & Risk Assessment
- Key regulatory risks by geography
- Fraud and trust risks
- Operational risk matrix
- Mitigation recommendations

### 10. Financial Position
- Funding history and investor analysis
- Comparable valuations
- Investment thesis analysis
- Financial health assessment

### 11. Team Assessment
- Founder-market fit evaluation
- Team completeness analysis
- Hiring signals and priorities
- Culture and organizational health

### 12. The Wedge & Strategic Assessment
- Wedge analysis (entry point, expandability, defensibility)
- Why now / why them analysis
- Bull case (3-5 key arguments)
- Bear case (3-5 key arguments)
- Base case scenario
- Strategic recommendations

### 13. Key Risks & Open Questions
- Top 10 risks ranked by severity and likelihood
- Unanswered questions that need primary research
- Information gaps and confidence levels

### 14. Appendix
- Data tables and charts
- Competitor comparison matrices
- Source list and methodology notes
- Glossary of terms

---

## QUALITY GUIDELINES FOR ALL AGENTS

1. **Be specific, not generic.** "The global real estate market is large" is useless. "$3.7 trillion in global residential real estate transactions annually" is useful.
2. **Cite or qualify everything.** If a number comes from a specific source, cite it. If it's an estimate, say so and explain your reasoning.
3. **Flag low-confidence claims.** If you couldn't verify something (like Criby's 1M monthly users claim), flag it explicitly.
4. **Think critically.** Don't just describe — analyze. What does this mean? Why does it matter? What's the implication?
5. **Compare to benchmarks.** Numbers without context are meaningless. Always compare to competitors, industry averages, or historical benchmarks.
6. **Identify the non-obvious.** Surface insights that aren't immediately apparent from looking at the website. What's hidden in the data?
7. **Be honest about gaps.** If you can't find information on something, say so clearly rather than padding with generic filler.
8. **Write for a decision-maker.** The audience is someone evaluating this company — as an investor, competitor, potential partner, or potential employee. Every sentence should help them make a better decision.
