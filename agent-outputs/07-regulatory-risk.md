## Regulatory, Legal & Risk Analysis: Criby (criby.com)

**Subject:** Criby -- Global multilingual real estate marketplace for buying/renting across 100+ countries
**Date:** 2026-05-25
**Analyst scope:** Regulatory, legal, and operational risk factors

---

### Executive Summary

- **Licensing fragmentation is the single largest regulatory barrier.** Real estate licensing is governed at the national (and often sub-national) level, with no global standard. Operating across 100+ countries means navigating regimes that range from strict state licensing (France, Germany, Dubai) to virtually unregulated markets, with the critical legal distinction between "marketplace/advertising platform" and "brokerage" determining whether a license is required at all.

- **Data privacy compliance is expensive and operationally complex at Criby's stated scale.** GDPR (EU), CCPA/CPRA (California), and strict data localization laws in China, Russia, and India each impose different -- and sometimes conflicting -- obligations. Cross-border data transfers for a 100+ country platform require a patchwork of adequacy decisions, Standard Contractual Clauses, and in some cases locally hosted infrastructure.

- **Financial regulations create material exposure if Criby handles payments.** Any escrow, deposit handling, or payment facilitation triggers money transmitter licensing (state-by-state in the US alone), AML/KYC obligations under FATF-aligned regimes, and potential OFAC sanctions screening requirements. A $4.7M OFAC penalty against a real estate investor in late 2025 signals escalating enforcement.

- **Fraud risk at global scale is severe and potentially existential.** FBI data shows US real estate fraud hit $275M in 2025 (up 59% YoY). One in five rental listings online is estimated to be fraudulent. A marketplace operating in 100+ countries with limited local verification infrastructure faces compounding fraud, trust, and liability risk.

- **Tax obligations multiply rapidly.** Digital services VAT/GST rules tightened globally from January 2026, with platforms increasingly treated as deemed suppliers. OECD Pillar One nexus thresholds, FIRPTA withholding on US property, and country-specific service fee taxation create a complex compliance matrix.

---

### Detailed Findings

#### 1. Real Estate Licensing Requirements

##### The Brokerage vs. Marketplace Legal Distinction

This is the threshold question for Criby's regulatory exposure. The distinction varies by jurisdiction:

**Pure advertising/listing platform (marketplace model):** If Criby only displays third-party listings and connects buyers/renters with sellers/landlords -- without negotiating deals, advising on price, or handling funds -- it may qualify as an advertising platform rather than a brokerage in many jurisdictions. This is the model used by Rightmove (UK), ImmobilienScout24 (Germany), and Idealista (Spain/Portugal/Italy).

**Brokerage model:** If Criby facilitates negotiations, provides valuations, handles escrow, or acts as an intermediary in the transaction, it would likely be classified as a brokerage and require licensing in most jurisdictions.

##### Country-Specific Licensing Requirements

**United States:**
- Real estate licensing is state-level. All 50 states plus DC regulate brokers independently.
- 41 states require firm registration for entities offering brokerage services.
- Average pre-licensing education: 99.8 hours, ranging from under 50 to over 150 hours.
- A designated broker must oversee all firm activities and is personally liable for agent conduct.
- Marketplace portals like Zillow operate under advertising/technology classification, not brokerage, which is why Zillow does not hold brokerage licenses in most states (though Zillow Homes, its iBuying arm, did).

**United Kingdom:**
- Estate agents do not need a license to operate. However, agents must belong to an approved redress scheme under the Consumers, Estate Agents and Redress Act 2007.
- Letting agents in Wales must be licensed. England does not yet require licensing for lettings agents, though the Renters' Rights Act 2025 is expanding tenant protections.
- Online portals like Rightmove and Zoopla are classified as advertising platforms, not estate agents.

**Germany:**
- Agents require a municipal permit under Section 34c of the German Trade Regulations (GewO).
- The regulatory regime is relatively strict, with required training and specialization.
- Property portals (ImmobilienScout24, Immowelt) operate as advertising platforms.

**France:**
- Among the most strictly regulated in Europe. Real estate professionals must hold a "carte professionnelle" (professional card) issued by the local Chamber of Commerce.
- Requires professional liability insurance, a financial guarantee, and ongoing professional development.
- Platform classification matters: advertising-only portals face fewer requirements, but any advisory or transactional role triggers full licensing.

**Dubai/UAE:**
- RERA (Real Estate Regulatory Agency) certification is mandatory for all real estate agents.
- Property portals require a RERA-approved license and must register on the Trakheesi system for advertising permits.
- Listings must use real photos and comply with DLD (Dubai Land Department) data privacy rules.
- Only UAE residents working with licensed brokerages can obtain RERA certification, making remote operation extremely difficult.

**Australia:**
- State-level licensing required for real estate agents. Foreign agents can apply for recognition in some states (e.g., Victoria).
- The Foreign Investment Review Board (FIRB) regulates all foreign property purchases, with application fees from AUD 14,100 to AUD 1M.
- Advertising foreign property to Australian buyers triggers additional disclosure requirements.

**EU-Wide Framework:**
- No EU-level harmonization of real estate licensing -- each Member State sets its own rules.
- CEPI (European Confederation of Real Estate Professionals) recommends 120 ECTS of education but has no enforcement power.
- The EU's European Crowdfunding Service Provider Regulation (ECSPR) applies if any investment/crowdfunding features are involved.

##### How Competitors Handle Multi-Jurisdiction Compliance

The dominant competitive pattern is **regional, not global, operation:**
- **Zillow** operates only in the US. Does not serve international markets.
- **Rightmove** primarily UK, with an "Overseas" section covering 90+ countries as advertising only.
- **Idealista** covers Spain, Portugal, and Italy -- three countries with similar legal traditions.
- **ImmobilienScout24** covers Germany, Austria.
- No major competitor attempts what Criby claims (active marketplace in 100+ countries). This is a significant competitive differentiation claim but also the source of the largest regulatory risk.

---

#### 2. Data Privacy & Protection

##### GDPR (European Users)

- Applies to any company processing personal data of individuals in the EEA, regardless of where the company is based.
- Requires explicit consent before collecting, storing, or processing personal data.
- Fines up to EUR 20 million or 4% of global annual turnover.
- Requires Data Protection Officer (DPO) appointment for large-scale processing.
- Cross-border transfers outside the EEA require adequacy decisions, Standard Contractual Clauses (SCCs), or Binding Corporate Rules (BCRs).
- Meta was fined EUR 1.2 billion in April 2023 for unlawful US data transfers -- a precedent that applies to any platform transferring EU user data.
- Real estate platforms must implement granular consent controls allowing tenants/clients to choose what data they share.

##### CCPA/CPRA (California)

- Applies to for-profit businesses with gross annual revenue over $26.625 million (as of January 2025), or those handling data of 100,000+ California residents.
- Six consumer rights: know, delete, opt-out, non-discrimination, correct, and limit sensitive data use.
- New requirements effective January 1, 2026: mandatory cybersecurity audits, risk assessments, and automated decision-making technology rules.
- Real estate-specific note: publicly available government property records are exempted from CCPA's definition of personal information.

##### Data Localization Requirements by Country

**China:** Critical information infrastructure operators must store all personal data on domestic servers. Cross-border transfers require a security assessment by the Cyberspace Administration. Penalties up to RMB 10 million (~USD 1.4M) for violations.

**Russia:** Federal Law No. 242-FZ requires all databases containing Russian citizens' personal data to be located on servers within Russia. Penalties range from RUB 60,000 to RUB 18 million, with potential website blocking for repeated violations.

**India:** The Digital Personal Data Protection Act (DPDP, 2023) with rules finalized November 2025 uses a negative-list model -- transfers are permitted unless the government specifically restricts a country. The Reserve Bank of India mandates all payment data be stored in India.

**Brazil:** LGPD requires standard contractual clauses approved by the national data protection authority for international transfers, with compliance mandatory since August 2025.

**Implication for Criby:** Operating in 100+ countries means potential data localization obligations in at least 4-6 major markets that require dedicated in-country infrastructure, dramatically increasing operational costs.

---

#### 3. Financial Regulations

##### Money Transmitter Licensing

- If Criby handles payments, deposits, or escrow on behalf of users, it likely requires a Money Transmitter License (MTL) in each US state where it operates.
- MTLs are issued state-by-state, with each state having different requirements, fees, and examination processes.
- Similar licensing regimes exist in the EU (Payment Services Directive/PSD2), UK (FCA authorization), and most major markets.
- Marketplace/crowdfunding platforms that hold buyer funds in escrow for sellers are explicitly identified as requiring MTLs.

##### AML/KYC Obligations

- Real estate is classified as a high-risk sector for money laundering globally under FATF (Financial Action Task Force) guidelines.
- FinCEN's Residential Real Estate Rule (effective date extended to March 1, 2026, currently vacated by court order but under appeal) would require reporting of beneficial owners in all-cash property transfers to legal entities.
- Australia is implementing new AML/CTF obligations for real estate agents effective July 1, 2026 (Tranche 2 reporting entities).
- EU's 6th Anti-Money Laundering Directive (6AMLD) imposes criminal liability for AML failures.
- KYC requirements include verifying buyer/renter identity, tracing source of funds, and screening against sanctions lists.

##### OFAC Sanctions Compliance

- OFAC administers US sanctions against targeted countries (Russia, Iran, North Korea, etc.), individuals, and entities.
- In November 2025, OFAC imposed a $4.7M penalty on an individual for purchasing real estate owned by a sanctioned Russian person -- the largest individual penalty in a public OFAC enforcement action.
- Any platform facilitating property transactions involving sanctioned persons, entities, or jurisdictions faces severe penalties.
- A 100+ country platform must screen every transaction party against OFAC's Specially Designated Nationals (SDN) list, EU sanctions lists, and equivalent UK/Australian lists.

##### Currency Exchange Regulations

- Cross-border property transactions involve significant currency risk (transaction risk, translation risk).
- If Criby facilitates currency conversion, it may trigger additional licensing as a money services business.
- Many countries restrict capital outflows for property purchases (China, India, Malaysia).

---

#### 4. Consumer Protection

##### Tenant Rights Variations

Consumer protection for renters varies dramatically across Criby's claimed 100+ country footprint:

**UK:**
- Deposits must be protected in one of three government-authorized Tenancy Deposit Protection schemes within 30 days of receipt.
- Deposits capped at five weeks' rent (under GBP 50,000 annual rent) or six weeks' rent (above).
- Landlords who fail to protect deposits can be ordered to pay 1-3x the deposit amount.
- The Renters' Rights Act 2025 significantly expands tenant protections in England.

**Germany:**
- Security deposits (Kaution) capped at 3 months' rent.
- Landlords must store deposits in a separate interest-bearing account.
- Landlords have 3-6 months to return deposits after tenancy ends.
- Strong tenant protections including limits on rent increases (Mietpreisbremse) in designated areas.

**France:**
- Buyers have a 10-day cooling-off period after signing a preliminary contract (compromis de vente), during which they can withdraw without penalty or reason.
- For rentals, deposits are capped at one month's rent (unfurnished) or two months (furnished).

**Australia:**
- Cooling-off periods vary by state: 5 business days (NSW, ACT), 3 business days (Victoria), 2 business days (South Australia), none (Western Australia for some transactions).
- Withdrawal penalties typically 0.25% of purchase price.

**EU General:**
- 14-day withdrawal right for distance/online contracts under EU Consumer Rights Directive 2011/83. However, this has explicit carve-outs for accommodation (non-residential purposes) and certain real estate services.

##### Disclosure Requirements

- Most jurisdictions require sellers to disclose known material defects, liens, and encumbrances.
- Requirements vary from strict statutory disclosure (US states, Australia) to caveat emptor principles (parts of Asia, Africa).
- A platform operating in 100+ countries cannot assume uniform disclosure standards.

---

#### 5. Platform Liability

##### Liability for Fraudulent Listings

**US -- Section 230 CDA:**
- Section 230 provides broad immunity for platforms from liability for third-party content (including listings).
- However, Section 230 does NOT protect platforms from liability for their own transactions (e.g., processing payments for illegal short-term rentals).
- If Criby curates, edits, or endorses listings, it may lose Section 230 protection.

**EU -- Digital Services Act (DSA):**
- The DSA (fully applicable since February 2024) imposes tiered obligations on online platforms.
- Marketplaces must verify seller identity before allowing listings (Know Your Business Customer).
- Platforms must enable easy reporting of illegal content and act on notices promptly.
- Annual content moderation transparency reports are mandatory.
- In 2025, the EU took enforcement action against Temu for failing to adequately vet illegal products -- precedent applicable to property listings.
- The DSA maintains conditional liability exemption (not broad immunity like Section 230).

**Other Jurisdictions:**
- Most countries lack clear platform liability frameworks for property listings.
- In many emerging markets, the platform may face strict liability for misrepresentations in listings.

##### Terms of Service Enforceability

- ToS enforceability across 100+ jurisdictions is extremely challenging.
- Mandatory consumer protection laws in the EU, UK, Australia, and elsewhere override ToS clauses.
- Choice-of-law and arbitration clauses may be unenforceable against consumers in their home jurisdictions.
- The EU Unfair Contract Terms Directive (93/13/EEC) renders many standard platform ToS clauses void.

##### Insurance Requirements

- US: Errors & Omissions (E&O) insurance required for licensed agents in Colorado, Louisiana, Montana, and others. Even where not legally required, it is industry standard.
- UK: Professional indemnity insurance required for property redress scheme membership.
- A platform positioning itself as a marketplace (not a brokerage) may not be legally required to carry E&O insurance, but the risk of claims from fraudulent or misrepresented listings makes it practically essential.

---

#### 6. Operational Risks

##### Fraud at Scale

**Quantified risk:**
- US real estate fraud losses: $275M in 2025, up 59% from $173M in 2024 (FBI).
- 12,368 real estate fraud complaints filed with the FBI in 2025 (up from 9,359 in 2024).
- One in five rental listings published online is estimated to be fraudulent.
- Craigslist's detection systems caught only 47% of fraudulent listings (NYU research).
- Real estate industry loses ~$500M annually to business email compromise (BEC) scams.
- More than 1 in 5 consumers report receiving suspicious communications during closing.

**Fraud vectors for a global marketplace:**
- Fake listings using stolen photos from legitimate listings or properties not owned by the lister.
- Identity fraud -- scammers impersonating owners, agents, or even law firms.
- Payment/wire fraud -- redirecting deposits or rent payments.
- Deepfake scams -- NAR has issued guidance on deepfake fraud in real estate as of 2025.
- Title fraud and property deed manipulation.

**Verification challenge at 100+ country scale:**
- No single identity verification system works across all jurisdictions.
- Property ownership records vary from digitized and public (US, UK, Australia) to paper-based, fragmented, or unreliable (many developing countries).
- Local language and legal system variations make automated verification extremely difficult.

##### Marketplace Trust Collapse Risk

- A global marketplace is only as strong as trust in its listings. A high-profile fraud incident in one market could damage trust globally.
- Unlike Amazon or Airbnb, real estate transactions involve life-altering sums, making each fraud incident highly damaging to reputation.
- Early detection recovers funds 73% of the time; delayed detection drops to 27% (CertifID data).

##### Supply Quality Control

- Verifying property condition, legal status, and ownership across 100+ countries requires local expertise that is extremely expensive to scale.
- Partnering with local agents/agencies introduces counterparty risk.
- Photo/video verification standards vary widely.

##### Geopolitical Risk

- Sanctions regimes (US/OFAC, EU, UK) restrict transactions involving Russia, Iran, North Korea, Syria, and others.
- Capital controls in China, India, Malaysia, and elsewhere restrict cross-border property purchases.
- Political instability in many emerging markets can freeze property markets overnight.
- War, civil unrest, and regime change can nullify property rights.

##### Currency Risk

- Exchange rate fluctuations between deal agreement and payment can materially alter transaction value.
- Transaction risk is especially acute for staged payments (deposit, balance, legal fees).
- Natural hedging (borrowing in the property's currency) is not available to all buyers.
- Forward contracts and currency options add cost and complexity.

---

#### 7. Tax Implications

##### Digital Services Tax / VAT / GST

- From January 2026, digital services VAT/GST rules tightened globally, with platforms increasingly treated as deemed suppliers responsible for collecting and remitting VAT/GST.
- Over 110 countries now impose VAT/GST on digital services.
- The OECD's International VAT/GST Guidelines recommend taxation at the customer's location.
- EU VAT applies to service fees charged by digital platforms to EU-based users.
- Platform service fees are subject to VAT/GST in most major markets.

##### Tax Nexus

- OECD Pillar One establishes nexus at EUR 1M revenue in a market jurisdiction (EUR 250K for smaller jurisdictions with GDP under EUR 40B).
- Pillar One's future is uncertain as of 2026 due to US non-cooperation.
- Many countries have implemented unilateral Digital Services Taxes (DSTs) in the interim -- India (6% equalization levy, though modified), UK (2% DST), France (3% DST), Italy (3% DST), Spain (3% DST).

##### FIRPTA (US)

- Foreign sellers of US real property face 15% withholding on gross sale price under FIRPTA.
- If Criby facilitates such transactions, it may have withholding agent obligations.
- Exception for buyer-occupied residences under $300,000.

##### Withholding Tax on Cross-Border Service Fees

- Many countries impose withholding tax on service fees paid to non-resident companies (typical range: 10-25%).
- Tax treaties may reduce or eliminate withholding, but treaty relief requires local filing and documentation.
- A platform receiving fees from 100+ countries faces a matrix of withholding obligations.

##### Tax Reporting Obligations

- OECD's Common Reporting Standard (CRS) requires financial institutions (and increasingly platforms) to report account information of non-residents to tax authorities.
- DAC7 (EU Directive on Administrative Cooperation) requires platforms to report seller/landlord income data to EU tax authorities -- effective January 2023.
- If Criby lists properties where landlords earn rental income, it may be a DAC7 reporting entity.

---

### Key Data Points

1. **$275 million** -- US real estate fraud losses in 2025 (FBI), up 59% YoY from $173M in 2024.
2. **1 in 5** rental listings published online is estimated to be fraudulent.
3. **EUR 20 million or 4% of global turnover** -- maximum GDPR fine for data protection violations.
4. **$4.7 million** -- largest OFAC penalty against an individual for real estate sanctions violation (November 2025).
5. **41 US states** require firm registration for real estate brokerage entities.
6. **110+ countries** now impose VAT/GST on digital services as of 2026.
7. **EUR 1.2 billion** -- Meta's GDPR fine for unlawful cross-border data transfers (April 2023).
8. **30 days** -- UK deadline to protect tenant deposits in a government-authorized scheme.
9. **10 days** -- France's mandatory cooling-off period for property buyers.
10. **15%** -- FIRPTA default withholding rate on gross sale price for foreign sellers of US property.
11. **85%** -- passing score required for RERA broker certification in Dubai.
12. **47%** -- percentage of fraudulent listings detected by Craigslist's own systems (NYU study).
13. **July 1, 2026** -- Australia's new AML/CTF obligations for real estate agents take effect.
14. **January 1, 2026** -- expanded CCPA cybersecurity audit and risk assessment requirements take effect.
15. **RMB 10 million (~$1.4M)** -- maximum penalty for data localization violations in China.

---

### Strategic Implications

#### Critical Path Items

1. **Legal structure classification is foundational.** Criby must establish and defend its classification as an advertising/marketplace platform (not a brokerage) in every jurisdiction where it operates. This is the single most impactful regulatory decision, as it determines whether licensing is required. Any feature that crosses into advisory, negotiation, or transaction facilitation territory risks reclassification.

2. **Phased geographic rollout is the only viable compliance strategy.** No competitor has successfully operated a licensed or compliant real estate marketplace across 100+ countries simultaneously. The claim of 100+ countries should be examined for how it is operationally delivered. If listings are user-generated with minimal platform involvement, the advertising platform classification is stronger. If the platform actively curates, verifies, or facilitates, per-country compliance becomes necessary.

3. **Data infrastructure must be architected for sovereignty.** China and Russia alone require dedicated in-country data storage. India's payment data localization adds another layer. A single global database architecture is incompatible with these requirements.

4. **Payment handling is a regulatory tripwire.** If Criby touches money at any point -- deposits, service fees collected from sellers, or payment facilitation -- it triggers financial licensing obligations in virtually every market. The safest approach is to redirect payments to licensed local partners, but this reduces platform control and revenue capture.

5. **Fraud prevention must be invested in disproportionately.** With 1 in 5 rental listings fraudulent and detection rates below 50% even on established platforms, a global marketplace without robust verification is a fraud incubator. Listing verification, identity verification, and payment protection are existential investments, not optional features.

6. **Sanctions compliance is non-negotiable and must be real-time.** OFAC, EU, and UK sanctions lists change frequently. Screening must be continuous, not one-time. The $4.7M OFAC penalty precedent in 2025 demonstrates that real estate is now firmly in the enforcement spotlight.

7. **Tax compliance at scale requires dedicated infrastructure.** DAC7 reporting, multi-country VAT/GST registration, DST compliance, and withholding tax management across 100+ countries requires either a dedicated tax operations team or partnership with a global tax compliance platform.

#### Risk-Reward Assessment

The regulatory burden of a truly global real estate marketplace is extreme. No existing competitor has attempted this scope. The dominant market pattern is regional specialization (Zillow = US, Rightmove = UK, Idealista = Southern Europe). Criby's 100+ country claim, if accurate and operationally real, represents either a genuine competitive moat built on significant compliance investment, or a significant regulatory risk if the compliance infrastructure does not match the geographic scope.

---

### Confidence Level

**Overall: MEDIUM-HIGH**

- **Licensing requirements (High confidence):** Well-documented regulatory frameworks; country-specific requirements are publicly available and verifiable.
- **Data privacy (High confidence):** GDPR, CCPA, and localization requirements are extensively documented and actively enforced.
- **Financial regulations (High confidence):** AML/KYC, MTL, and OFAC frameworks are well-established and recently reinforced with enforcement actions.
- **Consumer protection (Medium confidence):** Strong data for EU, UK, US, and Australia; limited data for many of the 100+ countries Criby claims to serve.
- **Platform liability (Medium-High confidence):** US Section 230 and EU DSA frameworks are clear; many other jurisdictions lack established precedent for property listing platforms.
- **Operational risks / fraud (High confidence):** FBI data, academic studies, and industry reports provide strong quantification.
- **Tax implications (Medium confidence):** Rapidly evolving landscape, especially OECD Pillar One uncertainty and unilateral DST proliferation.
- **Criby-specific compliance posture (Low confidence):** Criby.com provides minimal public information about its legal structure, licensing, compliance approach, or corporate entity. The platform's homepage offers limited detail beyond marketing claims.

---

### Sources & Methodology

**Methodology:** Multi-source web research covering regulatory frameworks, enforcement actions, industry analysis, academic studies, and competitor analysis. Research conducted May 2026 using public regulatory databases, legal publications, government resources, and industry reporting.

**Primary Sources:**

Regulatory & Legal Frameworks:
- [Harbor Compliance -- Real Estate Licensing](https://www.harborcompliance.com/real-estate-license)
- [GetLicenseMap -- How to Become a Real Estate Broker 2026](https://getlicensemap.com/blog/how-to-become-a-real-estate-broker)
- [Propertymark -- UK Regulation of Estate and Letting Agents](https://www.propertymark.co.uk/professional-standards/uk-regulation.html)
- [Schlun & Elseven -- Real Estate License Germany](https://se-legal.de/real-estate-lawyer-in-germany/real-estate-license-germany/?lang=en)
- [CEPI -- Real Estate Agents Regulation](https://cepi.eu/en/regulation)
- [GoDubai -- Dubai Real Estate Regulations for Brokers](https://www.godubai.estate/broker-hub/dubai-real-estate-regulations-for-brokers-dld-rera-rules/)
- [Dubai Land Department -- RERA](https://dubailand.gov.ae/en/rera)
- [Legal Advice Middle East -- UAE Property Listing Platform Permissions](https://legaladviceme.com/questions/104529/is-permission-required-to-operate-property-listing-platform-in-uae)

Data Privacy:
- [Secure Privacy -- GDPR Consent Management for Real Estate](https://secureprivacy.ai/blog/gdpr-consent-management-commercial-real-estate)
- [Secure Privacy -- Cross-Border Data Transfers 2025 Guide](https://secureprivacy.ai/blog/cross-border-data-transfers-2025-guide)
- [Secure Privacy -- CCPA Requirements 2026](https://secureprivacy.ai/blog/ccpa-requirements-2026-complete-compliance-guide)
- [California Attorney General -- CCPA](https://oag.ca.gov/privacy/ccpa)
- [FileCloud -- Data Residency Requirements by Country](https://www.filecloud.com/blog/data-residency-requirements/)
- [Captain Compliance -- Data Localization Laws by Country](https://captaincompliance.com/education/data-localization-laws-by-country/)
- [Recording Law -- Data Localization Laws by Country 2026](https://www.recordinglaw.com/world-laws/world-data-privacy-laws/data-localization-laws-by-country/)

Financial Regulations:
- [Klippa -- KYC & AML for Real Estate](https://www.klippa.com/en/blog/information/kyc-aml-real-estate/)
- [iDenfy -- KYC in Real Estate Compliance](https://idenfy.com/blog/kyc-aml-real-estate/)
- [InnReg -- Money Transmitter License Steps & Requirements 2026](https://www.innreg.com/blog/money-transmitter-license-steps-and-requirements)
- [FinCEN -- Residential Real Estate Rule](https://www.fincen.gov/rre)
- [Bradley -- FinCEN's New Real Estate Reporting Rule](https://www.bradley.com/insights/publications/2025/11/fincens-new-real-estate-reporting-rule-historical-context-compliance-requirements-legal-challenges)
- [Gadens -- New AML/CTF Obligations for Real Estate from July 2026](https://www.gadens.com/legal-insights/new-aml-ctf-obligations-for-real-estate-businesses-from-1-july-2026-its-time-to-start-getting-ready/)
- [Mayer Brown -- OFAC $4.7M Real Estate Penalty](https://www.mayerbrown.com/en/insights/publications/2025/11/ofac-announces-4-7-million-penalty-on-real-estate-investor-for-dealing-in-blocked-property-linked-to-russian-oligarch)
- [OFAC -- Basic Information on Sanctions](https://ofac.treasury.gov/faqs/topic/1501)

Consumer Protection:
- [Propertymark -- Tenancy Deposit Protection Explained](https://www.propertymark.co.uk/professional-standards/consumer-guides/tenants/tenancy-deposit-protection.html)
- [HousingAnywhere -- German Rental Laws and Tenant Rights](https://housinganywhere.com/Germany/tenant-rights-in-germany)
- [Landlord Knowledge -- TDP Rules, Schemes & Penalties 2026](https://landlordknowledge.co.uk/tenancy-deposit-protection-rules-schemes-penalties-2026-guide/)
- [Pinsent Masons -- Renters' Rights Act 2025 Guide](https://www.pinsentmasons.com/out-law/guides/renters-rights-act-2025-guide-private-landlords-england)
- [Parlez Moi De Paris -- French Real Estate Cooling-Off Period](https://www.parlezmoideparis.com/en/news/withdrawal-period-real-estate-buyers)
- [CommBank Australia -- Understanding Cooling Off Period](https://www.commbank.com.au/brighter/property/understanding-the-cooling-off-period.html)

Platform Liability:
- [EU -- Digital Services Act Impact on Platforms](https://digital-strategy.ec.europa.eu/en/policies/dsa-impact-platforms)
- [Compliance and Risks -- DSA Marketplace Accountability](https://www.complianceandrisks.com/blog/online-marketplaces-are-accountable-for-products-sold-on-their-platforms-eu-digital-services-act/)
- [MarketplaceRisk -- How Section 230 Protects Your Platform](https://www.marketplacerisk.com/post/how-section-230-protects-your-platform)
- [Dynamis LLP -- Section 230 Under Fire](https://www.dynamisllp.com/knowledge/section-230-immunity-changes)

Fraud & Operational Risk:
- [NAR -- Online Real Estate Fraud Climbed to $275M in 2025](https://www.nar.realtor/magazine/real-estate-news/online-real-estate-fraud-climbed-to-275m-in-2025-fbi-says)
- [Kiplinger -- Real Estate Scams 2025](https://www.kiplinger.com/real-estate/how-to-spot-and-avoid-real-estate-scams)
- [Group-IB -- The Reality of Deception: Real Estate Frauds](https://www.group-ib.com/blog/the-reality-of-deception-real-estate-scams/)
- [NAR -- Spotting Deepfake Scams in Real Estate](https://www.nar.realtor/the-facts/consumer-guide-spotting-deepfake-scams-in-real-estate)
- [Red Pin Company -- FX Risk Management for International Real Estate](https://www.redpincompany.com/insights/foreign-exchange-risk-management-international-real-estate)

Tax:
- [Tax Foundation -- Digital Taxation Around the World](https://taxfoundation.org/research/all/global/digital-taxation/)
- [Global VAT Compliance -- Digital Services VAT 2026](https://www.globalvatcompliance.com/globalvatnews/digital-services-vat-2026/)
- [Fonoa -- VAT & GST on Digital Services: Global Guide](https://www.fonoa.com/resources/blog/global-vat-and-gst-on-digital-services)
- [OECD -- Role of Digital Platforms in VAT/GST Collection](https://oecd.org/tax/beps/the-role-of-digital-platforms-in-the-collection-of-vat-gst-on-online-sales-e0e2dd2d-en.htm)
- [IRS -- FIRPTA Withholding](https://www.irs.gov/individuals/international-taxpayers/firpta-withholding)
- [Baker McKenzie -- Navigating the Digital Tax Landscape](https://www.bakermckenzie.com/en/insight/publications/2025/03/navigating-the-digital-tax-landscape)
