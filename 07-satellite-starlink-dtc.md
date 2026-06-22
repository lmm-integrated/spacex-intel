# 07 · Satellite business, Starlink & Direct-to-Cell (facts)

The actual cash engine. Starlink is the one clearly profitable leg of SpaceX and the foundation under the whole valuation.

## The constellation `[HIGH]`

- **12,342 satellites launched; ~10,687 in orbit; ~10,671 operational** (Jonathan McDowell catalog, 2026-06-22). Crossed 10,000 simultaneous active sats on 2026-03-17.
- Generation split: Gen1 ~3,291 operational (aging out); **Gen2 / V2 Mini ~7,380 operational** (the bulk); **Gen3 / V3: only 2 on orbit, both non-operational test units** (deployed on Starship Flight 12).
- FCC authorized up to **15,000** total (added 7,500 Gen2 in Jan 2026).
- **Direct-to-Cell: ~650 sats operational.**

## V3 generation `[MED]`

- **Launches on Starship only** (too large for Falcon 9). Stated specs: ~**1 Tbps downlink per sat** (~10x V2 Mini), optical laser links, enhanced Direct-to-Cell.
- **No operational V3 deployed yet.** Target to begin operational V3 batches **H2 2026**, now at schedule risk because Starship is grounded (see [04-starship-space.md](04-starship-space.md)). This is the single most important dependency in the growth story: V3 capacity underpins the post-IPO narrative, and it is gated on Starship returning to flight.

## Manufacturing & launch `[HIGH]`

- **~70 Starlink satellites/week** built in Redmond, WA (~3,640/yr). User terminals are built in **Bastrop, TX** (~15,000/day). (Common trap: Bastrop = terminals, Redmond = satellites.)
- **2025: 165 orbital launches** (6th straight annual record), **123 Starlink (~74.5%)**.
- **2026 YTD: ~69 Falcon launches by mid-June, >80% Starlink.**
- Booster reuse record: **B1067 = 35 flights**; ~626 successful landings of 639 attempts.

## Starlink commercial metrics `[HIGH, S-1]`

- **2025 revenue $11.39B** (~61% of SpaceX total, ~+50% YoY); Q1 2026 revenue $3.26B.
- **2025 adjusted EBITDA ~$7.17B (~63% margin)**; Q1 2026 $2.09B. **Starlink is strongly profitable** (do not confuse this with the net-loss-making parent).
- **10.3M subscribers** (end-Q1 2026), 160 countries. Blended **ARPU fell from ~$99 (2023) to ~$66 (early 2026)** as the mix shifted to lower-priced residential in more countries.
- First US residential price hike in years (June 2026): plans up $5-10/mo.
- Segments: maritime, aviation growing fast (United Airlines deal >1,000 aircraft). Quilty Space estimates ~$20B Starlink revenue / ~16.8M subs for 2026 `[MED: estimate, S-1 stops at Q1'26]`.

## Government & defense `[HIGH unless noted]`

- **Space Force "Backbone" (ex-MILNET): $2.29B firm-fixed-price OTA** (May 2026), a proliferated-LEO military comms layer feeding Golden Dome; prototype due end-2027.
- **NRO proliferated architecture:** ~14 dedicated launches by mid-June 2026, >150 sats since early 2025 (Starshield-built). Underlying ~$1.8B 2021 contract is Reuters-reported, not officially confirmed `[MED]`.
- **Golden Dome:** SpaceX is **1 of 12 firms** on space-based-interceptor prototype OTAs, combined ceiling up to $3.2B (SpaceX's individual slice undisclosed; $3.2B is a ceiling, not awarded cash). Demo deadline 2028.
- **NSSL Phase 3:** Lane 1 won 100% of task orders through May 2026 (~$1.55B); Lane 2 ~60% of the $13.7B structure.
- ~$22B lifetime federal commitments across NASA/DoD/Space Force `[MED]`.

## Direct-to-Cell (current + the spectrum pivot) `[HIGH unless noted]`

- **T-Mobile "T-Satellite with Starlink" commercially live since July 23, 2025.** Maturity ladder: text (2025) → picture/data (Oct 2025) → **voice calling in beta (late 2025)**. Coverage: continental US, PR, HI, parts of AK, plus Canada, NZ, Japan.
- Model today: MNO partnership using **partner terrestrial spectrum** (T-Mobile PCS). EchoStar/Boost added via the spectrum deal.
- **The strategic pivot, owned spectrum:**
  - **~$17B EchoStar deal (Sept 8, 2025):** AWS-4 + PCS H-block, **~50 MHz**, paid $8.5B cash + $8.5B SpaceX stock + ~$2B of EchoStar interest through Nov 2027.
  - **~$2.6B follow-on (Nov 6, 2025):** EchoStar's AWS-3 (15 MHz uplink, Band n70), all-stock.
  - This gives SpaceX **dedicated, licensed mobile spectrum it owns outright**, enabling a next-gen system targeting **5G/LTE-comparable connectivity from space**, not just partner-spectrum text.
- **Next-gen DTC capacity: >100x** the first-gen system (per-sat throughput ~20x via SpaceX silicon + phased arrays + owned spectrum, times a much larger fleet) `[MED]`.
- **>10M DTC MAU**, projected **>25M by end-2026** (S-1) `[MED]`.
- **No standalone DTC revenue line is broken out** in the S-1. Any DTC revenue figure circulating is inference.
- **Competitive fault line:** SpaceX/T-Mobile vs a consolidated **Amazon-Apple/Globalstar** (Amazon's ~$11.6B Globalstar acquisition, April 2026, includes Apple's stake; Amazon Leo D2D from 2028) vs **AST SpaceMobile** (AT&T/Verizon). D2D TAM ~$50B by 2030 `[LOW: single-tier estimate]`.

See [SOURCES.md](SOURCES.md) for citations. Forward-looking implications are in [08-forward-thesis-valuation.md](08-forward-thesis-valuation.md).
