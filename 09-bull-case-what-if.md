# 09 · Bull case: the "what-if" scenario & valuation runway (FORECAST + OPINION)

> **This is the most speculative file in the set.** It deliberately *assumes the bull what-ifs come true* and models the upside. It is not a base case or a prediction. Our own adversarial stress-test (below) rates most of these assumptions LOW-to-MEDIUM plausibility. Files 01-07 are facts; this is a conditional scenario. Not financial advice.

## The what-ifs, and how plausible they actually are

We red-teamed each assumption. The bull case requires the whole stack to hit; the stress-test says that's a long shot:

| What-if assumption | Stress-test plausibility | Why |
|---|---|---|
| SpaceX gets ~20% of early Vera Rubin capacity for early 2027 | **LOW** | The "20%" is one hedged podcast estimate (Altimeter's Clark Tang), no Nvidia/SEC confirmation; "early 2027 deployment" was never actually stated. |
| Grok reaches the frontier by September 2026 | **MEDIUM** | Grok 4.3 is #4 (~8 pts behind Opus 4.8); Grok 5 (6T) already slipped twice, ~45% odds it even ships before September. |
| Starship 13 & 14 succeed + prove Starlink V3 / reuse in 2026 | **LOW** | Ship reuse is gated on two perfect ocean landings; Flight 12 failed (booster crash, ship tipped). Two clean flights months apart plus a reuse milestone is a tall stack. |
| First Vera Rubin shipments fill Colossus 2 or a new site | **MEDIUM** | Rubin ships H2 2026 but is HBM4-constrained and back-half-loaded; Colossus 2 is already being filled with Blackwell. Rubin is a late-2026/2027 increment, not the fill. |
| Anthropic + Google renew past the 90-day windows | **LOW** | Both are self-described short-term bridges; both customers are aggressively building their own TPU/Trainium silicon. The S-1 itself warns the ~$26B could compress in 18-24 months. |

So read what follows as: *if the dice land right.*

### What each what-if actually requires (and the risk that breaks it)
- **20% Vera Rubin:** needs Nvidia to carve ~1-in-5 of its scarcest early Rubin units to a non-hyperscaler over CoreWeave/Oracle/Microsoft/Meta/OpenAI, SpaceX to confirm it (it hasn't), Rubin to ship early enough, and the sites to be liquid-cooling-ready for 1,800-2,300W GPUs. *Breaks if:* the figure is wrong, it's one hedged podcast estimate with the hedges stripped by aggregators.
- **Grok frontier by Sept:** needs Grok 5 (6T) shipping in usable, independently-verified form by ~July-Aug at or above Opus 4.8 / GPT-5.5, which are themselves iterating. *Breaks if:* schedule slips (already missed Q1 and Q2; ~45% odds before Sept).
- **Starship 13+14 + V3/reuse:** needs the FAA to clear Flight 12 fast, two clean flights months apart, and (for a ship catch) two perfect ocean landings first. *Breaks if:* cadence slips or any flight fails; the reuse precondition is one the program just failed.
- **Rubin fills Colossus 2:** needs Nvidia H2-2026 volume (HBM4-gated) AND a real early xAI allocation. *Breaks if:* it's just a late-2026/2027 increment, since Colossus 2 is already filling with Blackwell.
- **Lease renewals:** needs AI compute so tight that Google/Anthropic still can't self-supply, their own buildouts to slip, and pricing to hold. *Breaks if:* either exits at the Dec-31 window, both are explicitly building their own silicon and call the deals short-term bridges.

## Does a Vera Rubin purchase even show up in filings? (your question)

Mostly no, not where you'd expect:
- **SpaceX side:** the S-1 says SpaceX buys chips **purchase-order only, with no long-term binding orders**. A routine PO is therefore *not* a disclosable event. A *firm, material, non-cancellable* commitment would surface in the **"Commitments & Contingencies" footnote** of the **first post-IPO 10-Q (due ~late July to August 2026, for the quarter ending June 30)**, or in MD&A capex language, or in an 8-K only if it's a "material definitive agreement." Watch the Q2 10-Q.
- **Nvidia side:** only as an **anonymized ">10% customer"** ("Customer A/B/C/D") in the 10-Q, or as a *partner mention* in a Rubin keynote. Nvidia gives aggregate backlog ("$1T Blackwell+Rubin through 2027"), never a per-customer number.
- **Net:** if SpaceX has placed big Rubin POs, the cleanest tell will be the Q2 10-Q commitments footnote and the capex line, not a press release. As of now, SpaceX's disclosed GPU deals are about leasing capacity *out* (Anthropic/Google), not buying *from* Nvidia.

The bond (priced Jun 23 at $25B, IG-rated, ~$89B order book, ~$100.8B cash already on hand) is stated for refinancing the bridge loan plus "general corporate purposes," which is broad enough to fund GPU/datacenter capex even though that isn't the headline use.

## The bull flywheel (if the what-ifs hit)

1. **Starship returns to flight** (13/14 clean) and starts deploying **operational Starlink V3** (~1 Tbps/sat), which inflects Starlink capacity and revenue and de-risks AI1.
2. **Grok 5 (6T) ships to the frontier by September**, turning the AI segment from a ~$6B/yr cost center into a product business and a credibility unlock.
3. **Anthropic + Google renew**, converting ~$26B of "bridge" compute revenue into durable, high-margin recurring revenue.
4. **Vera Rubin lands** to fill Colossus 2's next phase / MACROHARDRR, adding a new ~$10-15B/yr compute line at premium, scarce-supply rates.
5. Each leg reinforces the others (launch funds satellites fund cash flow funds compute funds the model that fills the compute), and the "only vertically integrated AI company" narrative (Oppenheimer) gets *confirmed* rather than hoped.

## Revenue build under the full bull case `[FORECAST: estimates]`

| Segment | 2025A | 2026E (bull) | 2027E (bull) |
|---|---|---|---|
| Starlink | $11.4B | ~$20B | ~$32B |
| Space / launch | $4.1B | ~$5B | ~$7B |
| Grok / X (AI product) | $3.2B | ~$5B | ~$8B |
| Compute leasing | ~$0 | ~$14B | ~$38B |
| **Total** | **$18.7B** | **~$44B** | **~$85B** |

Notes: 2026 compute is a partial-year ramp (Anthropic ~8 mo + Google from Oct + Reflection from July). 2027 compute = renewals (~$28B) plus a new Vera Rubin line (~$10B). For reference, Arete's Street-high implies ~$66B of 2027 revenue, so this full-bull build (~$85B) is actually *above* the Street-high revenue assumption.

## The valuation runway `[OPINION: model]`

Baseline: ~$153/share (2026-06-29), ~$2.02T market cap, **13.17B shares** (use **~13.5B** post-Cursor close, ~+2.8% dilution). Price = revenue x P/S multiple / shares.

**End-2026, on ~$44B bull revenue:**

| Multiple | Market cap | Price/share | vs $165 |
|---|---|---|---|
| 40x | $1.76T | ~$130 | -21% |
| 55x | $2.42T | ~$179 | +9% |
| 70x | $3.08T | ~$228 | +38% |

(The market already pays ~50x 2026E here, so 2026 upside needs the multiple to *hold* high while revenue ramps.)

**End-2027, on ~$85B bull revenue:**

| Multiple | Market cap | Price/share | vs $165 |
|---|---|---|---|
| 25x | $2.1T | ~$158 | -4% |
| 35x | $3.0T | ~$221 | +34% |
| 50x | $4.3T | ~$315 | +91% |
| 62x | $5.3T | ~$390 | +136% |
| 80x | $6.8T | ~$504 | +205% |

**Read:** the credible bull 12-24 month runway is roughly **$250-400/share (~$3.3-5.3T)**, which lands on top of the Arete Street-high ($401 / ~$5.3T). It requires *both* the revenue roughly doubling to ~$85B *and* the market still paying a premium 35-62x sales multiple. Beyond 2027, if compute leasing scales with Rubin and Starship/V3 + Direct-to-Cell inflect, a ~$120-150B revenue base could support $4-6T+ even at a more normalized 30-40x.

For calibration, the full analyst spread: Arete $401 (~$5.3T), Oppenheimer $250 (~$3.3T), KGI $227, Wolfe $175, New Street $165 (spot), CFRA $115 (~$1.5T), Morningstar $63 (~$0.83T). Consensus ~$188 avg / $175 median. The independent SOTP (FutureSearch) pegs fair value at ~$1.25T, i.e., ~40% *below* spot.

## The double-bet problem (why the bull case is fragile)

- **It's a bet on revenue AND multiple simultaneously.** Even peak-Nvidia only ever sustained ~28x trailing P/S and has compressed to ~20x. SPCX needs a far higher multiple to *persist* while revenue 4-5x's. If the multiple normalizes toward 25-35x as growth is "proven," the stock can be roughly flat even if revenue doubles (see the 25x row).
- **The biggest revenue line is the most fragile.** Compute leasing (~$28-38B of the 2027 bull) is exactly the piece the stress-test rates LOW for durability: 90-day cancellable, with both customers building their own silicon. If Anthropic/Google exit at the Dec-31-2026 window, the bull revenue build loses its single largest incremental driver, and the S-1 warns xAI (burning ~$10B/yr) could face a cash squeeze.
- **Two of the flashiest inputs are unverified:** the 20% Rubin allocation (one hedged source) and ship reuse in 2026 (gated on a milestone the program just failed).

## Bottom line

If you grant every what-if, the model supports a **$250-400 share-price runway over 12-24 months (roughly +50% to +140%)**, converging on the Street-high. But that is a stacked, conditional bet: most of the load-bearing assumptions are rated LOW/MEDIUM, the largest revenue driver is cancellable, and you're betting a ~50-80x sales multiple survives the transition from story to numbers. The cleaner risk/reward is to treat the **Aug-Dec 2026 lockup unlocks** and the **Q2 10-Q + first 90-day lease window (post Dec 31)** as the moments that either confirm the flywheel or break it, and size any position to the fact that this is the speculative tail, not the base case.

_Analysis by Claude Opus 4.8, point-in-time 2026-06-29. Forecast and opinion, not facts; not financial advice; not a licensed advisor. See [08-forward-thesis-valuation.md](08-forward-thesis-valuation.md) for the balanced thesis and [SOURCES.md](SOURCES.md) for citations._
