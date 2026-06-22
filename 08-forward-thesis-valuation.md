# 08 · Forward thesis & valuation (INFERENCE + FORECAST + OPINION)

> **This file is NOT facts.** Files 01-07 are the sourced fact base. This file is what we *infer* and *forecast* from those facts, plus an opinionated valuation view. It is analysis, not a recommendation, and not personalized or licensed investment advice. Position sizing and the buy/sell decision are the reader's. Every number here is an estimate unless it links back to a fact file.

Three tiers, kept distinct:
- **INFER** = reasoned from the facts (high logical confidence, not separately sourced).
- **FORECAST** = scenarios about the future (genuinely uncertain).
- **OPINION** = our valuation call and entry view.

---

## INFER: where the compute is going and what it earns

**Where does Vera Rubin land?** The reported "~20% of early Vera Rubin capacity" is a single analyst's estimate (Altimeter's Clark Tang on BG2), not a disclosed contract, and the S-1 says SpaceX buys GPUs purchase-order only with no long-term supplier contracts. *If* it is directionally right, it almost certainly deploys into the **Colossus II next-phase expansion** (the S-1's stated "+220,000 GB300 / +400 MW" phase) and the **MACROHARDRR / Southaven build-out**, not a brand-new campus. Reasoning: no fourth site has been announced, the path to Musk's "almost 2 GW" runs through the existing Colossus II footprint, and Rubin slots in as the generation *after* the GB300 wave already going in there. So "new building?" -> no; "Colossus 2 future buildout?" -> yes, that's the most probable home.

**What can they monetize it at?** From the three signed leases (file 03), blended realized rates are roughly **$5,700/GPU/month (Anthropic, mixed) to ~$8,000+/GPU/month (Google/Reflection GB300-class)**. Vera Rubin is the scarcest, highest-performance silicon, so early Rubin capacity should command a **premium to GB300 rates** while supply is tight. INFER: a full Rubin hall (say ~100k GPUs) leased at GB300-plus rates is a **~$10-12B/year revenue line** at very high incremental margin, *if* they can fill it and customers don't cancel.

**Margins.** Because Colossus 1 was already built and ~89% idle, leasing it is ~80%+ contribution margin (file 03). INFER: that headline margin is **not repeatable on greenfield Rubin** capacity that has to be financed from scratch; it reverts toward the **45-70% neocloud band** (CoreWeave/Nebius). The bond and the IPO exist precisely because greenfield AI capex ($12.7B in 2025, ~$30B annualized) has to be funded up front.

**The speed moat.** SpaceX stood up clusters in 122 / 92 / (S-1-stated) 64 days vs ~15 months for typical rivals, via captive supply (Tesla Megapacks, in-house construction, behind-the-meter gas). INFER: this is a **real 6-18 month lead** and the genuine differentiator of the compute business. But it is **partly regulatory arbitrage** (unpermitted Memphis turbines drew legal challenge) and partly copyable (Stargate, Meta are going behind-the-meter too). So treat it as a durable-but-eroding edge, not a permanent moat.

---

## FORECAST: the revenue build

Directional scenarios, not predictions. 2025 actuals are the anchor (file 02/07).

| Segment | 2025 actual | 2026 forecast (base) | Driver / dependency |
|---|---|---|---|
| Starlink | $11.4B | ~$18-20B | subs 10.3M -> ~16-17M; price hikes; aviation/maritime; **V3 capacity gated on Starship** |
| Launch / Space | $4.1B | ~$4.5-5.5B | cadence + NSSL/NRO/Golden Dome backlog |
| AI: Grok product | ~$0.5-3.2B* | ~$2-4B | Grok 5 ship + X/Tesla integration |
| AI: compute leasing | ~0 | **~$15-28B run-rate** | Anthropic + Google + Reflection, **but 90-day cancellable** |

\*The S-1 reports the AI *segment* at $3.2B (includes X ads/data + Grok subs).

**The swing factor is compute leasing.** If the Anthropic/Google/Reflection leases run and more are signed, SpaceX's *consolidated* revenue could roughly double toward **$35-50B in 2026-2027**. If demand softens and tenants exercise the 90-day exits, that line is far smaller and far lumpier. This single dynamic is the difference between the bull and bear cases.

**What grows the pie beyond 2026 (optionality, low confidence):**
- **Starship working** unlocks V3 Starlink (>20x capacity/launch), cheaper constellation refresh, and the AI1 orbital-datacenter moonshot.
- **Direct-to-Cell on owned EchoStar spectrum** turns a partner-spectrum texting feature into a potential 5G-from-space line (no revenue broken out yet; TAM ~$50B by 2030).
- **Grok closing the frontier gap** (the 6T/10T bet) would make the AI segment a product business, not just a cost center filling Colossus.

---

## OPINION: valuation and entry view

**Where it trades (fact):** ~$166/share, **market cap ~$2.19T**, EV ~$2.44T, **~117-131x trailing sales**. For context that is ~6x the richest mega-cap multiple (Nvidia ~20x, Tesla ~15x, CoreWeave ~10x P/S).

**Our sum-of-the-parts peg (estimate):**
- **Starlink** ~$350-550B (high-growth, ~63% EBITDA-margin infrastructure on ~$20B forward revenue).
- **Launch / Space** ~$150-350B (dominant position, government backlog, Starship/Mars optionality).
- **AI (Grok + compute book)** ~$250B-1T (huge range: the leasing run-rate is large but cancellable and loss-making today; the last private xAI mark was ~$250B).
- **Facts-anchored total: ~$0.75-1.4T. With aggressive AI credit: ~$2-3T.**

So at **~$2.2T, the market is already pricing near-full execution** of the AI-compute + Starship + Direct-to-Cell trifecta. The profitable, growing Starlink engine and the verified multi-billion-dollar leases are real and support a large number, but probably **$0.9-1.4T on what exists today**. The gap to ~$2.2T is the forward bet.

**The analyst spread frames the debate:** Arete Buy **$401** (Street-high, V3/Starship thesis), Oppenheimer Outperform **$250** ("only vertically integrated AI company"), CFRA **Sell $115**, Jim Chanos openly short ("not worth $1.75T on any reasonable assumptions"), Morningstar fair value reportedly ~$63 `[unverified]`. That ~6x spread between bull and bear targets is itself the signal: this is a narrative stock where the valuation depends almost entirely on which forecast you believe.

**Is it an investment target / is this an entry?** Our view, clearly labeled opinion:
- **The business is assembling in the right direction.** Vertical integration (launch + the dominant satellite network + a frontier AI lab + a fast-to-build compute fleet) is genuinely unique, and the pieces reinforce each other.
- **But at ~120x sales it is priced for near-perfection,** and three of the load-bearing bull inputs are soft: the AI leases are 90-day cancellable, Starship is grounded (V3 and AI1 both wait on it), and Grok is behind the frontier. Two flashy bull data points (the 20% Vera Rubin allocation and the cheapest build-speed claims) are estimates, not confirmed.
- **Asymmetry today favors patience over chasing.** A disciplined approach is to **watchlist it and define an entry on weakness** rather than buy at the post-IPO high. Natural catalysts for a better entry: the **lockup-unlock waterfall (Aug-Dec 2026)** adds supply; and the thesis gets *confirmable* if (a) the compute leases survive past their first 90-day windows, (b) Starship returns to flight and starts deploying operational V3, and (c) Grok 5 actually ships and benchmarks competitively.
- If someone wanted exposure now, this profile (high-conviction story, extreme multiple, binary catalysts) fits a **small, speculative, high-volatility allocation**, not a core position, and explicitly not advice.

**Bottom line:** the *facts* justify a large, premium company (~$1T-ish). The *current price* requires you to also pre-pay for the AI-compute, Starship, and Direct-to-Cell futures largely working out. The pieces are growing in the right direction, but at ~$2.2T you are buying the forecast, not the facts. We would want either a cheaper entry or one of the three confirmations above before treating it as a high-conviction buy.

---

### Watchlist triggers (what would move our view)
- Compute leases renewed/expanded past 90-day windows -> bullish (margin durability proven).
- A tenant exercises the 90-day cancellation -> bearish (revenue quality questioned).
- Starship Flight 13/14 success + first operational V3 batch -> bullish (unlocks Starlink growth + AI1).
- Grok 5 (6T) ships and benchmarks at/above frontier -> bullish (AI becomes a product, not a cost center).
- Lockup unlocks (Aug 11, rolling through Dec 9) -> likely near-term supply/volatility, possible better entry.
- Bond pricing (coupon/size) -> reads on how the credit market prices the AI burn.

_Analysis by Claude Opus 4.8, 2026-06-22. Not financial advice; not a recommendation; we are not a licensed advisor. See files 01-07 for the underlying facts and SOURCES.md for citations._
