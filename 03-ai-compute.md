# 03 · AI compute (Colossus, GPUs, leases, Vera Rubin)

The ex-xAI Memphis-area datacenters are now SpaceX's AI backbone and its newest revenue line: SpaceX leases compute to its own rivals.

## GPU counts (raw chips) `[HIGH]` from the S-1

The S-1 (CIK 1181412) describes the clusters by build milestone, not headline totals. It never uses the strings "550,000 GPUs," "230,000 GPUs," or "H100-equivalent." Those come from Musk's X posts and trade press.

| Cluster | Raw GPUs / processors | Chips | Power |
|---|---|---|---|
| **Colossus 1** | ~220,000-230,000 | 150k H100 + 50k H200 + 30k GB200 | ~250-300 MW |
| **Colossus 2 (installed)** | ~220,000 | 110k GB200 + 110k GB300 | ~430 MW |
| **Colossus 2 (next phase, planned)** | +220,000 more GB300 | GB300 (Blackwell Ultra) | +400 MW |
| **Full Memphis-complex target** | ~550,000-555,000 | GB200 + GB300 | ~1.5-2 GW |

S-1 verbatim: Colossus first cluster ~100,000 H100 at ~130 MW (122 days). Colossus 2 first cluster ~110,000 GB200 / ~210 MW (91 days); second cluster 110,000 GB300 / 220 MW (64 days); next phase "at least 220,000 additional GB300 processors and over 400 additional megawatts." The Anthropic lease describes Colossus 1 as ~222,000 GPUs (H100/H200/GB200), 300+ MW.

**Ambiguity flag `[MED]`:** the "550,000" figure is not clean. SemiAnalysis counts it at the **NVL72 node level** (2 GPUs/node → implies >1M GPUs); Introl treats it as raw GPUs. The S-1 never uses it. Treat 550k as an aggregate/marketing full-buildout target, not a verified installed count.

## H100-equivalents `[LOW: computed, not published]`

No primary source publishes a current H100-equivalent total. The only official H100-equiv figure is Musk's **5-year forward target of "50 million H100-equivalent" (~200 exaFLOPS)**, not current capacity.

Using Nvidia's multiplier (GB200 ≈ 4x H100 for LLM training, ~5x raw FLOPS; GB300 a bit higher):

| | Raw | ≈ H100-equivalent |
|---|---|---|
| Colossus 1 (~230k, mostly Hopper) | 230k | **~340k-370k** |
| Colossus 2 installed (~220k Blackwell) | 220k | **~880k-1.1M** |
| Colossus 2 + next phase (~440k) | 440k | **~1.8M-2.2M** |
| Full 555k target | 555k | **~2.2M-2.8M** |

**This is our arithmetic, not a sourced figure.** The takeaway that matters: Colossus 2 is where the real compute is. Similar raw chip count to Colossus 1, but **~3x the H100-equivalent compute** because it's all Blackwell. That's exactly why xAI moved Grok training to Colossus 2 and leased the Hopper-heavy Colossus 1 out.

## The compute leases (SpaceX as landlord)

xAI's Colossus 1 had an "embarrassingly low" ~11% training utilization on its mixed-GPU architecture (per a memo from xAI president Michael Nicolls), so Grok training moved to the all-Blackwell Colossus 2 and the stranded Colossus 1 capacity got leased out.

- **Anthropic (Colossus 1)** `[HIGH]`: announced 2026-05-06. Anthropic rents **all** of Colossus 1 (300+ MW, ~220,000 GPUs), paying **$1.25B/month through May 2029** (~$40-45B headline). Triggered the May 2026 Claude Code rate-limit increases (doubled the 5-hour limits, removed peak-hour throttling for Pro/Max). The irony: Musk had called Anthropic/Claude "misanthropic and evil" in Feb 2026, then approved the lease in May saying "No one set off my evil detector." Anthropic also said it has "expressed interest in partnering with SpaceX to develop multiple gigawatts of orbital AI compute" (i.e. AI1). Source: Anthropic's own post; SpaceX S-1.
- **Google (Colossus)** `[HIGH]`: disclosed 2026-06-05 via SEC filing. **Google pays SpaceX ~$920M/month, Oct 2026 to June 2029 (~$30B), for ~110,000 units** (note: mixes GPUs + CPUs + memory). Google is the *customer* (bridge capacity for Gemini Enterprise), not a provider. Source: SpaceX Free Writing Prospectus; TechCrunch.
- **Reflection AI (Colossus 2)** `[HIGH]`: reported 2026-06-22 by CNBC ("materials viewed by CNBC"). The open-source AI startup (last valued ~$25B pre-money) gets immediate **GB300** access and pays **$150M/month from July 1, 2026 through 2029 (~$6.3B)**. Reflection works with the DOE Genesis Mission and Pentagon AI efforts; the strategic angle is open-source/"American open intelligence." Note: this broke via CNBC, not an official @SpaceX post. Source: CNBC.
- The S-1's Anthropic cloud agreements are scoped at **~325,000 Nvidia GPUs across both sites** (tenant figure, distinct from installed cluster counts).

**Customer roster (4 external compute tenants):** Anthropic ($1.25B/mo), Google ($920M/mo), Reflection ($150M/mo), plus Cursor (which SpaceX is acquiring). Combined headline run-rate is **~$2.3B/month (~$28B/year)** if all run full term, but every lease carries the 90-day mutual-cancellation clause.

### Implied monetization `[LOW: our math]`
- Anthropic: $1.25B/mo ÷ ~220,000 GPUs ≈ **~$5,700/GPU/month** (mixed Hopper/Blackwell).
- Google: $920M/mo ÷ ~110,000 units ≈ ~$8,400/unit/month (but the unit count blends GPU+CPU+memory, so not directly comparable).
- Reflection: $150M/mo for undisclosed GB300 count. At a ~$8,000/GB300/mo assumption that implies ~18,000-19,000 GB300s.
- For reference, public neocloud H100 rental runs ~$2-3/GPU-hr (~$1,500-2,200/mo). SpaceX's blended rates look healthy, and because Colossus 1 was already built and ~89% idle, the contribution margin on that lease is estimated at **80%+** (reverts toward the 45-70% neocloud band on greenfield-financed capacity).

**Caveat `[HIGH]`:** Musk characterized the Anthropic deal as "a 180-day lease with 90-day mutual cancellation." Both leases reportedly carry 90-day mutual exit clauses, so the multi-year "$40B / $30B" totals are soft run-rate figures, not locked commitments.

### Lease renewal risk (the single biggest swing factor) `[HIGH]`

- **The 90-day cancellation windows become exercisable after Dec 31, 2026.** Q1 2027 is the first real renew-or-cancel signal.
- **Both customers are building their own silicon during the very window these leases run.** Anthropic has locked up 5 GW+ of Google/Broadcom TPU capacity (~1 GW in 2026 scaling to 3 GW+ in 2027) plus up to 5 GW of Amazon Trainium; Google owns the TPU stack itself and called its SpaceX deal "short-term" bridge capacity for a Gemini demand spike.
- **The S-1 explicitly warns** that if Google and Anthropic execute their own buildouts, the ~$26B combined compute revenue could compress within 18-24 months, and that xAI (burning ~$10B/yr) could face a cash crisis if the Anthropic contract terminates.
- Near-term (through 2026) GPU scarcity supports the leases holding; the structural risk is post-2026 substitution to in-house ASICs/TPUs. So the bull case (file 09) lives or dies on whether these convert from bridges into multi-year commitments, which none of the three parties has signaled.

## Vera Rubin commitment: the ~20% is real, but it's an analyst's channel check `[MED→LOW]`

The number you're reaching for exists, but its provenance is softer than "SpaceX committed to X%":

- **Origin:** Altimeter's **Clark Tang on the BG2 podcast** (Gerstner/Gurley), verbatim: *"as we gear up for the Vera Rubin chips, my conversations suggest they have secured perhaps up to 20% of that capacity, especially in the early days when these chips are incredibly scarce."* That is hedged channel-check intelligence ("my conversations suggest... perhaps up to"), **not a disclosed contract**. No dollar value, no unit count, no rack count.
- **The S-1 cuts against a hard commitment:** Risk Factors state *"We do not have any long-term or other material contractual arrangements with our direct chip suppliers, instead procuring all of our GPUs on a purchase-order basis."* So there is **no reserved Vera Rubin allocation in the filing.**
- **Nvidia** names "SpaceXAI" as a Vera Rubin adopter (alongside CoreWeave, Azure, Lambda) but publishes **no per-customer percentage.**
- **Timing:** Vera Rubin (VR200 / Vera Rubin NVL72) hit full production per CES Jan 2026; first samples shipped ~Feb 2026; volume ships H2 2026 ("this fall"). But it is **HBM4-constrained** (SK Hynix reportedly slipped its HBM4 ramp Q2->Q3 2026; TrendForce cut Rubin's 2026 share from 29% to 22%), so broad availability is "Q4 2026 at the earliest." Earliest realistic xAI Rubin deployment is late 2026/2027. Colossus 2 today is Blackwell (GB200/GB300), not Rubin.

**Honest framing:** an Altimeter partner *estimates* SpaceX/xAI has informally locked up to ~20% of early, supply-constrained Vera Rubin output, on the thesis they can stand up compute faster than anyone. Credible market intelligence, but not a committed or disclosed figure, and the S-1 says SpaceX holds no long-term supplier contracts.

### Would a Vera Rubin purchase even show up in filings? `[HIGH]`

Mostly no, not where you'd expect. Because the S-1 says SpaceX buys chips purchase-order-only with no long-term binding orders, a routine PO is **not** a disclosable event. A firm, material, non-cancellable commitment would surface in:
- the **"Commitments & Contingencies" footnote** of the **first post-IPO 10-Q** (Q2 2026, quarter ending June 30, due ~late July to August 2026), or MD&A capex language;
- an **8-K** only if it is a "material definitive agreement" (Item 1.01), which a routine PO is not.
- On **Nvidia's side**: only as an anonymized ">10% customer" ("Customer A/B/C/D") in its 10-Q, or a partner mention in a Rubin keynote. Nvidia gives aggregate backlog ("$1T Blackwell+Rubin through 2027"), never a per-customer figure.

So the cleanest tell that SpaceX has committed to big Rubin volume will be the **Q2 10-Q commitments footnote and the capex line**, not a press release. As of now, SpaceX's disclosed GPU dealings are about leasing capacity *out*, not committed purchases *from* Nvidia.

## "Colossus 3" and MACROHARDRR: no, it's not a third Colossus `[HIGH]`

**There is no "Colossus 3."** The S-1 defines exactly two AI facilities (zero occurrences of "Colossus 3/III"):

- **COLOSSUS** = flagship on Paul R. Lowry Road, Memphis TN (ex-Electrolux factory).
- **COLOSSUS II** = defined verbatim as *"our data centers in Memphis, Tennessee and in Southaven, Mississippi"* (Tulane Road, Memphis + Stateline Road, Southaven).

So the **MACROHARDRR site is the Southaven leg of Colossus II, not a separate Colossus 3.** That 810,258-sq-ft warehouse at 2400 Stateline Road West (bought ~Dec 2025 by MZX Tech LLC, the xAI/SpaceX subsidiary) is the "third building" Musk tweeted about, but it rolls up under Colossus II. They are **not breaking ground on a new "Colossus 3" campus**; the path to Musk's "almost 2 GW" runs through expanding the existing Colossus II footprint plus the stated next-phase GB300 expansion. No fourth/new campus has been announced as of 2026-06-22.

- Provenance: the 810,258-sq-ft former GXO Logistics warehouse was bought by **MZX Tech LLC** (a Wyoming entity at xAI's Palo Alto SEC address) from an affiliate of **ElmTree Funds (BlackRock-owned)**; the deed lists a **$10 placeholder** (Mississippi is a non-disclosure state, so the real price is not public). MZX had earlier bought a nearby ~114-acre former Duke Energy power-plant site (mid-2025) for supporting power. "MACROHARD" was also painted on the Colossus 2 roof in Memphis (Oct 2025), branding not a separate building.
- Mississippi permitted **41 natural-gas turbines** for the site (since challenged in court by the NAACP). Gov. Reeves announced it Jan 8 2026 as **$20B+**, the largest economic-development project in state history. First-phase ops targeted Feb 2026.

### Reality-check on capacity `[HIGH]`

- The S-1 says Colossus + Colossus II *"collectively provide approximately 1.0 gigawatt"* installed as of filing, versus Musk's "almost 2 GW" target.
- Independent satellite analysis (Epoch AI via Tom's Hardware, Jan 2026) put Colossus 2's actual installed **cooling at only ~350 MW**, well below advertised 1 GW. As with GPU counts, announced runs well ahead of operational.

See [SOURCES.md](SOURCES.md) for full citations.
