## Business Model & Monetization Deep Dive

### Executive Summary

- **Criby operates a hybrid freemium + transaction fee model**, charging landlords a tiered subscription (Free/Pro/Enterprise at COP 0 / ~$45 / ~$183 per month) with declining commission rates (10% / 5% / custom), plus a 5-10% tenant booking service fee. This dual-sided fee structure mirrors Airbnb's split-fee approach but at lower rates suited to long-term rental economics.
- **At 1M monthly users with realistic conversion assumptions (1-2% booking rate, ~$1,200 average monthly rent, 7.5% blended take rate), Criby's implied annual GMV is $144M-$288M, yielding $10.8M-$21.6M in gross revenue.** This positions them in early-growth territory comparable to Spotahome circa 2021-2022.
- **The biggest revenue upside sits in ancillary financial services** (deposit alternatives, rent insurance at $3-15/month, currency exchange) and B2B corporate relocation packages -- a $21.7B market growing at 7.2% CAGR. These could 2-3x the core marketplace take rate over time.
- **Criby's 100+ country footprint creates a severe cold-start/liquidity challenge.** With 50K listings across 100+ countries, average density is ~500 listings per country -- far below the threshold needed for reliable matching. Geographic concentration strategy is critical.
- **Unit economics are speculative but directionally viable.** If CAC can stay below $50-80 (organic/SEO-heavy acquisition for a multilingual platform), and average customer LTV reaches $90-180 (single transaction + insurance upsell), the LTV:CAC ratio of ~2-3x is survivable for early stage but needs improvement toward the 3:1+ benchmark.

---

### Detailed Findings

#### 1. Revenue Model Analysis

**Criby's Confirmed Pricing Structure (from criby.com/pricing):**

| Component | Free Plan | Pro Plan | Enterprise Plan |
|---|---|---|---|
| Monthly Cost | COP 0 (~$0) | COP 193,550 (~$45/mo) | COP 786,050 (~$183/mo) |
| Listings | Up to 3 | Unlimited | Unlimited |
| Commission on Transactions | 10% | 5% | Custom (negotiated) |
| Analytics | Basic | Advanced | Advanced + Custom |
| Verification | Standard | Premium badge | Premium + Custom |
| Featured Listings | None | 3/month | Unlimited |
| Support | Email | Priority | Dedicated account manager |
| Additional | Mobile app access | Virtual tour hosting, Lead mgmt tools | API access, White-label, SLA |

**Tenant-Side Fees:**
- Searching and applying: Free
- Service fee on bookings: 5-10% of transaction value
- Optional insurance: $3-15/month

**Competitor Fee Comparison:**

| Platform | Tenant Fee | Landlord Fee | Model Type |
|---|---|---|---|
| **Criby** | 5-10% booking fee | 5-10% commission (tier-dependent) | Hybrid: subscription + transaction |
| **HousingAnywhere** | 25-40% of first month's rent (min EUR 175) | 8% of total contract value | Transaction-only |
| **Spotahome** | Variable booking fee (undisclosed %) | Variable % of total contract value | Transaction + optional subscription plans |
| **Airbnb** | ~14.2% guest fee (split model) OR 0% (host-only model) | 3% (split) OR 15.5% (host-only) | Transaction-only |
| **Zillow** | Free | $200-$40,000+/month (ad-based, per ZIP) | Advertising/lead-gen |

**Analysis:** Criby's fee structure is significantly lower than HousingAnywhere's on the tenant side (5-10% vs. 25-40% of first month rent), which is a strong competitive advantage for cross-border tenants who are already bearing relocation costs. The tiered landlord model incentivizes professional landlords to upgrade for lower commission rates -- a proven SaaS upsell mechanic. However, the low absolute subscription price (COP-denominated, roughly $45-183/month) suggests the platform may be initially targeting Latin American or emerging markets where property managers operate at lower margins.

**Best-Fit Model Assessment:** The hybrid approach makes strategic sense for Criby's positioning:
- Transaction fees capture value from each successful match (aligned incentives)
- Subscription tiers create recurring revenue and reduce churn among professional landlords
- The free tier solves the supply-side cold-start problem
- Optional insurance creates embedded fintech revenue

This mirrors the evolution path of Spotahome (which moved from pure transaction fees to subscription tiers) and adds Zillow-style featured listing monetization.

---

#### 2. Potential Revenue Streams (Ranked by Near-Term Viability)

**Tier 1 -- Core (Live Today):**

1. **Tenant Booking Service Fees (5-10%):** Primary demand-side revenue. At blended 7.5% on a $1,200 average monthly rent, this yields $90 per transaction. For annual leases, this could compound if applied to total contract value.

2. **Landlord Commission (5-10%):** Supply-side transaction revenue. The tiered structure encourages volume -- professional landlords managing 10+ properties will upgrade to Pro to cut commission from 10% to 5%.

3. **Landlord Subscription Revenue:** Recurring SaaS revenue at ~$45-183/month. Even at modest penetration (5-10% of active landlords on paid plans), this creates predictable baseline revenue.

**Tier 2 -- Near-Term Expansion (6-18 Months):**

4. **Featured/Promoted Listings:** Already included in Pro (3/month) and Enterprise (unlimited). Standalone featured listing purchases for Free-tier landlords at $5-15/listing/week could add meaningful revenue. Benchmark: Zillow's rental advertising grew 41% YoY in Q3 2025 to $174M quarterly.

5. **Rent Insurance / Tenant Protection:** Already offered at $3-15/month. This is a high-margin embedded fintech product. The global rent deposit insurance market is $3.2-3.8B (2024) growing at 16-17% CAGR. At 10% attachment rate on 1M users, this is $360K-$1.8M/year in recurring premium revenue.

6. **Deposit Alternatives:** Replacing traditional security deposits (typically 1-2 months rent) with insurance-backed guarantees. HousingAnywhere charges 3% of Total Contract Value for their Rent Guarantee. For a 12-month lease at $1,200/month, that is $432 per tenant -- high-margin revenue with strong value proposition.

**Tier 3 -- Medium-Term (12-36 Months):**

7. **Corporate Relocation Packages (B2B):** The corporate relocation services market was valued at $21.68B in 2026, growing at 7.2% CAGR. Enterprise accounts with multinational companies relocating employees could yield $5,000-$50,000+ annual contracts. Even 10 enterprise clients at $25K/year = $250K in high-margin B2B revenue.

8. **Lead Generation for Local Services:** Connecting verified tenants with movers, furniture rental, utility setup, local insurance. Revenue model: cost-per-lead ($5-25) or revenue share (10-20%). High intent + known move date = premium lead quality.

9. **Currency Exchange / Cross-Border Payments:** International tenants paying rent across currencies. Margin on FX spread (1-3%) on monthly rent payments. At $1,200/month rent with 2% FX margin = $24/month per cross-border tenant. With 70+ languages and 100+ countries, this is native to Criby's value proposition.

**Tier 4 -- Long-Term (24+ Months):**

10. **Data & Analytics Products:** Rental market intelligence, pricing optimization tools for landlords, market reports for institutional investors. Comparable to CoStar/Zillow data products.

11. **Advertising Platform:** Display ads from moving companies, furniture retailers, insurance providers, visa services. High-intent audience (actively relocating) commands premium CPMs ($15-40).

12. **Mortgage/Financing Referrals (Buy Side):** For property purchases, referral fees to mortgage brokers/lenders. Zillow Mortgages generated $145M in 2024 revenue. Even at tiny scale, mortgage referrals at $500-2,000 per funded loan are lucrative.

---

#### 3. Unit Economics Modeling

**Key Assumptions:**

| Metric | Conservative | Base Case | Optimistic |
|---|---|---|---|
| Monthly Active Users | 1,000,000 | 1,000,000 | 1,000,000 |
| Visitor-to-Booking Conversion | 0.5% | 1.0% | 2.0% |
| Monthly Transactions | 5,000 | 10,000 | 20,000 |
| Average Monthly Rent (Global Blend) | $800 | $1,200 | $1,500 |
| Average Lease Duration (months) | 6 | 9 | 12 |
| Blended Take Rate (both sides) | 10% | 15% | 18% |

*Note: Blended take rate combines tenant fee (5-10%) + landlord commission (5-10%). At Pro-tier landlord (5%) + midrange tenant fee (7.5%) = 12.5% blended. Adding insurance attachment pushes toward 15-18%.*

**Implied Revenue (Annual):**

| Scenario | Monthly GMV | Annual GMV | Annual Gross Revenue |
|---|---|---|---|
| Conservative | $4.0M | $48M | $4.8M |
| Base Case | $12.0M | $144M | $21.6M |
| Optimistic | $30.0M | $360M | $64.8M |

**Customer Acquisition Cost (CAC) Estimates:**

| Channel | Estimated CAC | Notes |
|---|---|---|
| Organic SEO (multilingual) | $5-15 | Criby's 70+ language support is a massive organic moat; long-tail keyword opportunity in 100+ local markets |
| Content Marketing | $10-25 | City guides, relocation content, how-to articles |
| Paid Search (Google) | $40-80 | Real estate keywords are competitive ($2-8 CPC); 1-3% conversion to booking |
| Social/Meta Ads | $30-60 | Targeting expats, digital nomads, students |
| Partnerships (universities, employers) | $15-30 | Lower CAC through institutional channels |
| Referrals | $10-20 | Incentivized referral programs |
| **Blended CAC** | **$25-50** | **Weighted toward organic given multilingual SEO advantage** |

*Context: Industry-wide CAC jumped 40-60% between 2023-2025 due to privacy changes and competition. Real estate digital CAC benchmarks range from $50-$200+.*

**Lifetime Value (LTV) Estimates:**

| Segment | Single Transaction Revenue | Repeat Rate | Insurance Upsell | Estimated LTV |
|---|---|---|---|---|
| Short-term Renter (3-6 mo) | $60-$90 | Low (0.3x/yr) | $9-45 | $70-$135 |
| Mid-term Renter (6-12 mo) | $90-$180 | Medium (0.5x/yr) | $18-90 | $120-$300 |
| Long-term / Relocator | $150-$300 | Medium (0.5x/yr) | $36-180 | $200-$600 |
| Landlord (Free tier) | $60-$120/transaction | 2-5 transactions/yr | N/A | $120-$600/yr |
| Landlord (Pro tier) | $540/yr subscription + lower commission | Recurring | N/A | $800-$1,500/yr |
| B2B / Corporate | $5,000-$50,000/yr | Recurring | N/A | $15,000-$150,000/yr |

**LTV:CAC Ratio Projections:**

| Segment | LTV | CAC | LTV:CAC | Assessment |
|---|---|---|---|---|
| Short-term Renter | $70-$135 | $25-$50 | 1.4-5.4x | Marginal to good |
| Mid-term Renter | $120-$300 | $25-$50 | 2.4-12x | Strong |
| Landlord (Pro) | $800-$1,500/yr | $100-$200 | 4-15x | Excellent (SaaS economics) |
| B2B / Corporate | $15K-$150K | $1,000-$5,000 | 3-150x | Exceptional if closed |

**Path to Contribution Margin Positive:**
- Transaction fees alone (at 15% blended take rate on $1,200 rent) yield $180 per match
- If blended CAC is $40 per acquired user and conversion is 1%, effective CAC per transacting user = $4,000
- This math only works if: (a) organic/free channels dominate acquisition (driving blended CAC per transacting user below $200), (b) repeat usage and landlord subscriptions amortize acquisition costs, (c) insurance/fintech attach rates reach 15%+
- Comparable: Spotahome reached EBITDA profitability in H2 2024 at ~$65M revenue run-rate

---

#### 4. Marketplace Economics

**The Chicken-and-Egg Problem:**

Criby faces an acute version of the classic two-sided marketplace bootstrapping challenge, amplified by geographic breadth:

**Scale of the Problem:**
- 50,000 listings across 100+ countries = ~500 listings per country average
- In major cities (where demand concentrates), density might be 50-200 listings
- A functional rental marketplace needs 500-2,000+ listings per metro to feel "liquid"
- At 1M monthly users across 100+ countries = ~10,000 users per country = poor match density in most markets

**Which Side to Subsidize:**
Supply (landlords) should be subsidized first. Rationale:
- The Free tier (up to 3 listings, no upfront cost) already does this
- Landlords are the scarcer resource in international rental markets
- Each landlord listing serves multiple potential tenants (1-to-many ratio)
- Aggregating listings from existing platforms (a la early Airbnb) can simulate supply
- Landlords who list for free have zero switching cost -- retention requires booking volume

**Recommended Cold-Start Strategies:**
1. **City-by-city launch (not country-by-country):** Focus on 10-20 high-demand expat/relocation cities (Lisbon, Barcelona, Berlin, Amsterdam, Dubai, Mexico City, Bali/Canggu, Bangkok, Bogota, Buenos Aires) before spreading thin
2. **Aggregate existing supply:** Scrape or API-integrate listings from local platforms to inflate perceived inventory
3. **Seed demand through partnerships:** University exchange programs, corporate relocation firms, digital nomad communities
4. **Single-player mode:** Make the platform valuable to landlords even without tenants (analytics, listing management, virtual tour hosting)
5. **Set hard subsidy budgets:** Define liquidity milestones (e.g., 1,000 listings in a city, 50 bookings/month) that trigger monetization activation

**Liquidity Metrics to Track:**

| Metric | Target (Healthy) | Criby Estimated Current |
|---|---|---|
| Listings per active city | 500-2,000+ | ~200-500 (top cities) |
| Search-to-inquiry rate | 2-5% | Unknown |
| Inquiry-to-booking rate | 10-25% | Unknown |
| Time-to-fill (median days) | 7-21 days | Unknown |
| Matches per listing per month | 2-5+ | Unknown |
| Repeat booking rate | 15-30% annually | Unknown |

---

#### 5. Pricing Strategy

**Current Positioning vs. Competitors:**

Criby is positioned as the **low-cost, high-breadth** option:
- Tenant fees (5-10%) are 60-80% cheaper than HousingAnywhere (25-40% of first month)
- Landlord listing is free (vs. paid-only on many platforms)
- Geographic coverage (100+ countries) exceeds all named competitors
- COP-denominated pricing suggests LatAm origin/focus

**Pricing Psychology for International Users:**
- COP denomination may confuse or deter non-LatAm users; should offer USD/EUR/local currency display
- The $45/month Pro plan is extremely competitive globally -- possibly too cheap for developed markets (landlords in London/NYC would pay $200+/month without blinking)
- Consider geographic pricing tiers: Emerging Markets ($20-50/mo), Developed Markets ($75-200/mo), Premium Markets ($150-400/mo)
- The 10% commission on Free tier is competitive with traditional agent fees (one month rent / 10-15% annual) and positions upgrade to Pro (5%) as compelling

**Recommended Tier Structure Evolution:**

| Tier | Current | Recommended Evolution |
|---|---|---|
| **Free** | 3 listings, 10% commission | Keep as-is; essential for supply acquisition |
| **Pro** | ~$45/mo, 5% commission | Regionalize pricing; add more featured listings; introduce lead scoring |
| **Enterprise** | ~$183/mo, custom commission | Add white-label, API, dedicated support; position for property management companies and corporate relocation |
| **NEW: Premium Agent** | N/A | $300-500/mo; lead routing priority, CRM integration, co-branded marketing; targets professional agents/brokers |

**Free vs. Freemium Analysis:**
The current Free tier (3 listings) is well-calibrated:
- Allows individual landlords with 1-2 properties to participate without friction
- Creates a natural upgrade trigger at 4+ properties
- The 10% commission on Free tier means Criby still earns from every transaction
- Risk: if most transactions happen on Free tier, subscription revenue stalls

---

#### 6. Revenue Projections

**Based on 1M Monthly Users -- Scenario Analysis:**

**Scenario A: Low Monetization (Year 1-2)**
- 0.5% booking conversion = 5,000 bookings/month
- $800 average rent, 6-month average lease
- 10% blended take rate (mostly Free-tier landlords)
- Annual Revenue: **$4.8M**
- Plus insurance ($3-15/mo, 5% attach): +$180K-$900K
- Total: **~$5-6M**

**Scenario B: Base Case (Year 2-3)**
- 1.0% booking conversion = 10,000 bookings/month
- $1,200 average rent, 9-month average lease
- 12.5% blended take rate (mix of tiers)
- Annual Revenue: **$18M**
- Plus insurance (10% attach): +$720K-$3.6M
- Plus landlord subscriptions (2,000 Pro + 100 Enterprise): +$1.3M
- Plus featured listings: +$500K
- Total: **~$20-23M**

**Scenario C: Optimistic (Year 3-5)**
- 2.0% booking conversion = 20,000 bookings/month
- $1,500 average rent, 12-month average lease
- 15% blended take rate (premium mix)
- Annual Revenue: **$54M**
- Plus insurance (15% attach): +$2.7M-$13.5M
- Plus landlord subscriptions (5,000 Pro + 500 Enterprise): +$3.8M
- Plus B2B corporate (50 accounts at $25K): +$1.25M
- Plus ancillary (ads, FX, leads): +$2M
- Total: **~$64-75M**

**Comparable Marketplace Revenue Milestones:**

| Company | Revenue Milestone | When | Users/Scale at Time |
|---|---|---|---|
| Spotahome | $17M annual | 2022 | ~500K monthly users |
| Spotahome | $65M annual | 2025 | ~1.5M monthly users (est.) |
| HousingAnywhere | $5-25M annual (est.) | 2024 | EBITDA-profitable |
| Zillow Rentals | $453M annual | 2024 | 50K multifamily properties |
| Airbnb | $11B+ annual | 2024 | $81.8B GBV, ~9-13% take rate |

**Implied Valuation Range (if raising):**
- At $20M revenue and 8.8x PropTech revenue multiple = ~$176M valuation
- At $65M revenue and 8.8x multiple = ~$572M valuation
- Early-stage (pre-revenue or $5M) with strong growth = $30-80M on forward multiples

---

### Key Data Points

1. Criby charges landlords 5-10% commission (tier-dependent) plus tenants 5-10% booking fee, creating a 10-20% theoretical blended take rate
2. HousingAnywhere charges tenants 25-40% of first month's rent (min EUR 175) and landlords 8% of total contract value -- significantly more expensive than Criby on the tenant side
3. Airbnb's take rate is approximately 9.3-13.2% of GBV (varies by quarter), generating $11B+ annual revenue on $81.8B in 2024 GBV
4. Zillow's Rentals segment grew 41% YoY to $174M in Q3 2025 alone, driven by multifamily advertising
5. Spotahome reached $65.3M revenue in 2025 and hit EBITDA profitability in H2 2024 after exceeding EUR 200M in rental volume
6. The global rent deposit insurance market is $3.2-3.8B (2024) growing at 16-17% CAGR -- a natural adjacent revenue stream for Criby
7. Corporate relocation services market valued at $21.68B in 2026, growing at 7.2% CAGR
8. PropTech CAC benchmarks range from $50-$10,000; digital ad costs rose 5.13% market-wide, and CAC jumped 40-60% between 2023-2025
9. PropTech revenue multiples average 8.8x in 2025, reflecting premium over general SaaS
10. Healthy rental marketplace conversion benchmarks: 1.5-3% inquiry rate, 2-5% view-to-inquiry ratio, with top performers like Zillow exceeding 5%
11. At 50K listings across 100+ countries, Criby averages ~500 listings per country -- well below the 500-2,000+ per city needed for marketplace liquidity
12. Criby's Pro plan at ~$45/month is priced for emerging markets; developed-market landlords would accept 3-5x this price point
13. HousingAnywhere raised $50.7M total, valued at approximately $36.1M (down from $50M+) despite reaching EBITDA profitability
14. Average European apartment rent: EUR 1,900-2,300/month in top cities (Amsterdam, Rome, Paris); U.S. averages significantly higher
15. 1M monthly users at 1% conversion and $1,200 average rent with 15% blended take rate implies ~$21.6M annual revenue

---

### Strategic Implications

**1. Pricing is a Competitive Weapon but Leaves Money on the Table**
Criby's 5-10% tenant fee is dramatically cheaper than HousingAnywhere's 25-40%. This is a strong acquisition lever for price-sensitive international renters (students, expats, digital nomads). However, developed-market landlords are accustomed to paying more, and the COP-denominated pricing signals a narrow geographic focus. Regionalized pricing could capture 2-3x more revenue in premium markets without losing emerging-market competitiveness.

**2. The Liquidity Problem is Existential**
With 50K listings spread across 100+ countries, the marketplace is likely too thin in most individual cities to reliably match tenants with suitable properties. The "Planet Earth" branding is aspirational but operationally dangerous -- a marketplace that shows 12 listings in Berlin feels worse than one that shows 2,000 in Berlin. Recommendation: ruthlessly prioritize 15-20 cities and achieve density before geographic expansion.

**3. Fintech is the Margin Multiplier**
Transaction fees on rental marketplace are inherently thin (5-15% of relatively low-frequency transactions). The real margin comes from embedded financial services: deposit alternatives (one-time fee of 3% of total contract value), rent insurance ($3-15/month recurring), and cross-border FX (1-3% spread on every monthly payment). HousingAnywhere's Rent Guarantee and Spotahome's All-in plan demonstrate this path. These products could 2-3x Criby's revenue per user without increasing CAC.

**4. B2B Corporate Relocation is the High-LTV Play**
Individual tenant transactions have modest LTV ($70-$300). Corporate relocation accounts have $15K-$150K LTV. Even a small B2B sales team closing 20-50 enterprise accounts/year would generate $500K-$2.5M in high-margin recurring revenue and provide demand-side liquidity in key corporate markets (London, Singapore, Dubai, NYC).

**5. The Subscription Upsell Funnel Needs Work**
Moving landlords from Free (10% commission) to Pro (5% commission at $45/month) only makes economic sense for the landlord when their monthly commission savings exceed $45. At $1,200/month rent, the landlord saves 5% = $60/month on commission, netting $15/month. This is a thin value proposition. Either increase Free-tier commission, reduce Pro pricing, or add more Pro-exclusive features (analytics, lead scoring, CRM) to strengthen the upgrade incentive.

**6. Path to Profitability is Plausible but Requires Discipline**
Spotahome proved that a mid-term rental marketplace can reach EBITDA profitability at ~$65M revenue. Criby's lower fee structure means it needs higher volume or stronger ancillary monetization to match. The key lever is organic acquisition through multilingual SEO -- if 70+ language support translates into low-CAC organic traffic, the unit economics work. If Criby has to buy its way to 1M users through paid channels, the math gets very difficult.

---

### Confidence Level

**Overall: MEDIUM (6/10)**

- **High confidence (8/10):** Competitor pricing data (HousingAnywhere, Airbnb, Zillow) is from official sources and SEC filings
- **High confidence (8/10):** Criby's own pricing structure was extracted directly from criby.com/pricing
- **Medium confidence (6/10):** Revenue projections are model-based using industry conversion benchmarks; actual Criby conversion rates are unknown
- **Medium confidence (5/10):** CAC estimates are extrapolated from industry benchmarks, not Criby-specific data
- **Low confidence (4/10):** Criby's actual financial performance, funding status, and real user/traffic numbers are unverified. The "1M monthly users" claim could not be independently validated
- **Low confidence (3/10):** Spotahome's exact tenant booking fee and landlord commission percentages are not publicly disclosed, limiting direct comparison precision
- **Note:** Criby's about page lists leadership (Sarah Chen, Marcus Rodriguez, Elena Kowalski, David Park) and a 2024 founding date, but no funding, investors, or revenue were disclosed. The COP-denominated pricing and limited public profile suggest this is a very early-stage company.

---

### Sources & Methodology

**Primary Sources:**
- Criby.com -- About page and Pricing page (direct extraction)
- HousingAnywhere.com -- Tenant pricing, landlord pricing, and help center articles
- Spotahome.com -- Plans page and help center articles
- Zillow SEC filings (Form 8-K FY2024, FY2025 quarterly reports)
- Airbnb SEC filings (Form 8-K FY2024, FY2025 quarterly reports)
- Airbnb Help Center -- Service fee documentation

**Secondary Sources:**
- Tracxn -- HousingAnywhere and Spotahome funding data
- CB Insights -- Company financial profiles
- Online Marketplaces -- HousingAnywhere EBITDA reporting, Spotahome funding rounds
- GetLatka -- Spotahome revenue data ($65.3M, 2025)
- Coherent Market Insights -- Corporate Relocation Service Market sizing
- Growth Market Reports / DataIntelo -- Rent Deposit Insurance Market sizing
- First Page Sage / Phoenix Strategy Group -- CAC benchmarks by industry and channel
- Qubit Capital -- PropTech SaaS valuation and KPI benchmarks
- Financial Models Lab -- Marketplace KPI benchmarks
- Sharetribe -- Marketplace glossary (liquidity, chicken-and-egg definitions)
- NFX -- 19 tactics for marketplace cold-start
- Lodgify / Hostaway / FutureStay -- Airbnb fee structure documentation
- Prime Pixel Digital / HousingWire / TheClose -- Zillow Premier Agent pricing analysis
- GlobalPropertyGuide / HousingAnywhere Rent Index -- Global rental price benchmarks

**Methodology:**
1. Web research across competitor pricing pages, SEC filings, and industry databases
2. Direct extraction from Criby's public-facing pricing and about pages
3. Revenue modeling using industry-standard conversion rate benchmarks (1-3% for real estate marketplaces) and publicly available competitor metrics
4. Unit economics modeling using PropTech CAC/LTV benchmarks from venture databases
5. Cross-referencing marketplace economics frameworks from Sharetribe, NFX, and Cobbleweb
6. All currency conversions approximate using mid-2026 rates (COP 4,300 = $1 USD)
