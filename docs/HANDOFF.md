# Premium pet store: strategy and build handoff

Last updated 15 October 2026. Everything decided and built so far, in one place.

## 1. The business

- **What:** a premium UK pet store (dogs first, cats second), dropshipped, sold through a Shopify back end with a custom headless front end.
- **Positioning direction:** design-led beds, furniture and walk gear that look good in the home and stand up to British weather. Working idea: "from the wet walk to the warm room".
- **Markets:** UK first, built to expand worldwide. Prefer suppliers with warehouses in several regions (UK, EU, US) so products can move to new markets without re-sourcing.
- **Channel:** Google Ads first (Shopping and feed-only Performance Max). Meta later for brand content and retargeting.
- **Brand name:** not chosen. "Fell & Fireside" is a stand-in in the designs.

## 2. Decisions made

| Decision | Choice | Why |
|---|---|---|
| Legal entity | Ltd company, registered once funds allow, before any Google account is opened | Google Ads, Merchant Center and Shopify Payments all start under the company's identity, so nothing needs switching or re-verifying later |
| Storefront | Headless: Shopify back end, Hydrogen (React) front end on Oxygen hosting | Full design freedom for motion and custom layout; adapts easily with AI-written code; chosen for longevity over speed |
| Design direction | Direction 2 (clean, rounded, moving; based on a Motion Sites template) preferred over Direction 1 | More modern. Agreed it is still generic; refine once real products exist |
| Samples | No sampling by default; rely on supplier vetting rules (section 6) and track refunds per supplier | Cost. Accepting some refunds as part of the process |
| Product niche | Premium pet. Avoid food, treats, supplements, flea or medicinal products, shock collars, cheap electricals and medical claims | Regulation, safety and Google policy |

## 3. Strategy taken from the reference videos (and what was rejected)

Videos reviewed: Emrys "$1k/day with Google Ads + Shopify", Romas Ecom "AI dropshipping" and "Google Ads algorithm explained".

**Keeping:**
- Google Shopping for buyer intent; the product feed is the targeting. Titles follow: adjective, product, who it's for, selling points, use cases, specs, built from Google Keyword Planner terms.
- Merchant Center readiness: consistent business name, address and phone everywhere; original policies (shipping, returns, privacy, terms) with working contact links; About and FAQ pages; no fake urgency or fake "was" prices; 5–15 products at first, then a slow drip of new products.
- Performance Max set up feed-only: search and shopping focus, location "presence" only, TV screens off, asset enhancements off, no ROAS target in the first months, budget raises of 20% or less, weekly clean-up of search terms and non-selling products.
- Product research: seasonal, evergreen and trending products, checked with Google Trends and Keyword Planner, plus competitor best-seller lists.
- An automation pipeline (import, images, SEO and pricing, product page content), but every stage writes to **drafts** for approval, never straight to live.

**Rejected:**
- Duplicating one product into several listings to fill multiple ad slots ("surface area scaling"). Breaks Google's Unfair Advantage policy and risks account suspension; misleading under UK consumer law.
- Buying followers, running ads only to fake traffic, or "humanising" AI copy to slip past review.
- Fake reviews. Banned in the UK under the DMCC Act since 6 April 2025.
- Cloning a competitor's store content or catalogue images; lightly reworded copied policies.
- AI images that change the product itself. Generate the scene, keep the product accurate to the supplier photo.

## 4. Timeline

- **Now (low cost):** brand name and domain, supplier shortlist, headless build, automations.
- **When funds allow:** register the Ltd (£100 online), business bank account, business email, 020/03 phone number, Shopify plan (any standard paid plan includes Hydrogen/Oxygen; Basic is enough; build on a free development store until then), publish the site. Merchant Center wants the store live about 14 days before applying.
- **Launch:** Merchant Center, Google Ads (Organisation account), manual CPC warm-up, then feed-only Performance Max with a product drip.
- **Realistic ads start: January.** Christmas demand ends before then, so the launch range targets January–March demand.

## 5. Product research (15 October 2026)

Full interactive shortlist: https://claude.ai/artifact/53h1izfji8Nk4AwzkeYtYD
Raw data in this repo: `docs/research/shortlist.csv`, `docs/research/trends_uk_5y.csv`.

**Seasonal findings (UK Google Trends, five years):**
- "Dog bed" is the biggest term; peaks in November and holds at the yearly average through January–March. "Orthopedic dog bed" +47% year on year.
- "Dog car seat cover" peaks in February (+56% year on year). "Dog drying coat" runs 16% above average in January–March (+36%).
- "Dog sofa" +46%, "dog towel" +68%, "lick mat" +37% and peaks in January. "Puppy" peaks in January.
- Christmas terms (advent calendar, Christmas jumper, stocking) fall to almost zero from January to March.

**Shortlist (12 products, costs are estimates to confirm with suppliers):**

| Product | Role | Price | Landed cost | Profit before ads | Break-even ROAS | Stock |
|---|---|---|---|---|---|---|
| Orthopaedic memory-foam bolster bed | Hero | £109 | £58.04 | £48.53 (45%) | 2.25 | UK |
| Plush bolster sofa bed (bouclé/teddy look) | Hero | £69 | £23.01 | £44.36 (64%) | 1.56 | Abroad |
| Wall-mounted cat shelves set | Hero (cats) | £139 | £66.62 | £69.35 (50%) | 2.00 | UK |
| Dog car seat bed (small dogs) | Core | £74 | £38.99 | £33.28 (45%) | 2.22 | Abroad |
| Waterproof back-seat cover and extender | Core | £49 | £24.69 | £23.08 (47%) | 2.12 | UK |
| Boot liner with bumper flap | Core | £44 | £13.47 | £29.40 (67%) | 1.50 | Abroad |
| Hooded microfibre drying robe | Core | £36 | £10.44 | £24.59 (68%) | 1.46 | Abroad |
| Waterproof chew-resistant crate bed | Core | £59 | £28.97 | £28.60 (48%) | 2.06 | UK |
| Raised cat/small-dog sofa | Core | £79 | £39.09 | £38.08 (48%) | 2.07 | UK |
| Padded winter jacket (small dogs) | Seasonal | £32 | £7.38 | £23.73 (74%) | 1.35 | UK |
| Felt cat cave | Add-on | £39 | £16.56 | £21.41 (55%) | 1.82 | Abroad |
| Lick mat and slow-feeder set | Add-on | £19 | £6.75 | £11.62 (61%) | 1.64 | Abroad |

Assumptions: card fees 2% + 25p; UK-stock delivery assumed free (to confirm); no VAT (below the threshold at launch); ad spend not included.

**Competitors on Google Shopping UK:**
- **PawLunova:** Lake District-named beds (Ambleside, Grasmere, Elterwater), bouclé and memory foam, £69–139. Validates the "fell" positioning; a Lake District brand name would need to look clearly different.
- **By Teddy:** design-led bouclé/puffer pieces; car seat £95–115.
- **FunnyFuzzy:** best-sellers are dog car seat beds (£60–80) and sofa covers.
- **MyPetsworth:** best-sellers are chew-proof waterproof beds and crate mats (£30–55).
- **Silver Circle Pets:** a bouclé dog bed is their number one seller.
- **Charley Chau, Earthbound:** UK-made ceiling for the category (blankets, tweed beds, leather collars).

**Open gaps:**
- No bouclé bed with real sales history on AliExpress. The signature bouclé look needs a private supplier on 1688 or Alibaba, likely through a sourcing agent.
- Drying robe, boot liner and lick mat have no good UK-stock listings yet. CJ Dropshipping (UK/US/EU warehouses) needs a free account and a human check in Chrome before it can be searched.

## 6. Supplier vetting rules (no-sample approach)

- Recent customer photo reviews (last 60 days); 4.7+ rating with real order volume; supplier store 2+ years old.
- Specific specs (foam density, fabric weight, exact dimensions); vague listings are a red flag.
- Compare the same factory product across sellers; the cheapest is usually the downgraded one.
- UK warehouse stock with a stated handling time; multi-region warehouses preferred for expansion.
- Ask agents for photos or video of the actual unit before dispatch.
- Track refunds and complaints per product and per supplier from day one; pull anything over a set threshold.

## 7. Build status

- **Repository:** github.com/antoniomarktucker-design/storefront. Hydrogen (TypeScript) scaffold on mock.shop demo data; builds and type-checks. Claude GitHub App installed for push access.
- **Design canvas:** https://claude.ai/artifact/PAoUiCb8MXo3myzMYHprY7
  - Direction 1: "from the wet walk to the warm room" (Young Serif + Schibsted Grotesk, fell green, limewash, ember accent).
  - Direction 2 (preferred): Motion Sites template layout adapted to the store; vertical photo marquees, gradient-border buttons (pastel / "fell and ember" / monochrome options), collection carousel, FAQ accordion. No fake review badge.
- **Images:** five lifestyle images generated in Higgsfield (wet spaniel on a fell, spaniel by a wood burner, Labrador in a drying robe, cat on a sage sofa, bouclé zip detail). Higgsfield plan is in a grace period with a daily generation cap.
- **Connectors:** Shopify connector not yet authorised (connect once a store exists). Gmail, Google Drive, Higgsfield, Motion Sites and Claude in Chrome are available.

## 8. Planned automation system

All writes go to drafts for approval.
- **Product research (weekly):** trends, competitor best-sellers, candidate products with ratings, cost and UK delivery times, into a tracker for approval.
- **Listing pipeline (on approval):** Higgsfield scene images from supplier photos, keyword titles and descriptions, product page sections, slow drip before Merchant Center approval.
- **Orders (daily report):** new orders, unfulfilled after 48 hours, missing tracking, refunds, margin per order, drafted customer email replies. Fulfilment through the supplier's Shopify app; supplier payments stay with Antonio.
- **Ads (weekly, after launch):** search terms, wasted spend, budget steps of 20% or less.
- **Review layer:** a critical review of store performance, the systems and decisions, not a yes-man.

## 9. Next steps

1. Pick which shortlist products to keep, cut or swap.
2. Create a CJ Dropshipping account (complete its human check) so UK-warehouse versions can be checked; source bouclé options through a 1688/Alibaba agent.
3. Choose the brand name; check UKIPO (classes 18 and 20), Companies House, then register the .com and .co.uk. Shortlisted: Mews & Hound, Fell & Fireside, Kip & Hound, Ramble & Rest, Wilder & Warm (.com and .co.uk free as of 14 October).
4. Proof of concept on the headless build before design work: Merchant Center feed with the custom site's URLs, purchase conversion tracking, cookie consent.
5. Rebuild Direction 2 with real products, then refine away from the generic look.
