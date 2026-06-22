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

xAI's Colossus 1 had an "embarrassingly low" ~11% training utilization on its mixed-GPU architecture, so Grok training moved to the all-Blackwell Colossus 2 and the stranded Colossus 1 capacity got leased out.

- **Anthropic (Colossus 1)** `[HIGH]`: announced 2026-05-06. Anthropic rents **all** of Colossus 1 (300+ MW, ~220,000 GPUs), paying **$1.25B/month through May 2029** (~$40-45B headline). Triggered the May 2026 Claude Code rate-limit increases. Source: Anthropic's own post; SpaceX S-1.
- **Google (Colossus)** `[HIGH]`: disclosed 2026-06-05 via SEC filing. **Google pays SpaceX ~$920M/month, Oct 2026 to June 2029 (~$30B), for ~110,000 Nvidia GPUs.** Google is the *customer* (bridge capacity for Gemini Enterprise), not a provider. Source: SpaceX Free Writing Prospectus; TechCrunch.
- The S-1's Anthropic cloud agreements are scoped at **~325,000 Nvidia GPUs across both sites** (tenant figure, distinct from installed cluster counts).

**Caveat `[HIGH]`:** Musk characterized the Anthropic deal as "a 180-day lease with 90-day mutual cancellation." Both leases reportedly carry 90-day mutual exit clauses, so the multi-year "$40B / $30B" totals are soft run-rate figures, not locked commitments.

## Vera Rubin commitment: the ~20% is real, but it's an analyst's channel check `[MED→LOW]`

The number you're reaching for exists, but its provenance is softer than "SpaceX committed to X%":

- **Origin:** Altimeter's **Clark Tang on the BG2 podcast** (Gerstner/Gurley), verbatim: *"as we gear up for the Vera Rubin chips, my conversations suggest they have secured perhaps up to 20% of that capacity, especially in the early days when these chips are incredibly scarce."* That is hedged channel-check intelligence ("my conversations suggest... perhaps up to"), **not a disclosed contract**. No dollar value, no unit count, no rack count.
- **The S-1 cuts against a hard commitment:** Risk Factors state *"We do not have any long-term or other material contractual arrangements with our direct chip suppliers, instead procuring all of our GPUs on a purchase-order basis."* So there is **no reserved Vera Rubin allocation in the filing.**
- **Nvidia** names "SpaceXAI" as a Vera Rubin adopter (alongside CoreWeave, Azure, Lambda) but publishes **no per-customer percentage.**
- **Timing:** Vera Rubin (VR200 / Vera Rubin NVL72) hit full production per CES Jan 2026; volume ships H2 2026 ("this fall"). Earliest realistic xAI Rubin deployment is late 2026/2027. Colossus 2 today is Blackwell (GB200/GB300), not Rubin.

**Honest framing:** an Altimeter partner *estimates* SpaceX/xAI has informally locked up to ~20% of early, supply-constrained Vera Rubin output, on the thesis they can stand up compute faster than anyone. Credible market intelligence, but not a committed or disclosed figure, and the S-1 says SpaceX holds no long-term supplier contracts.

## "Colossus 3" and MACROHARDRR: no, it's not a third Colossus `[HIGH]`

**There is no "Colossus 3."** The S-1 defines exactly two AI facilities (zero occurrences of "Colossus 3/III"):

- **COLOSSUS** = flagship on Paul R. Lowry Road, Memphis TN (ex-Electrolux factory).
- **COLOSSUS II** = defined verbatim as *"our data centers in Memphis, Tennessee and in Southaven, Mississippi"* (Tulane Road, Memphis + Stateline Road, Southaven).

So the **MACROHARDRR site is the Southaven leg of Colossus II, not a separate Colossus 3.** That 810,258-sq-ft warehouse at 2400 Stateline Road West (bought ~Dec 2025 by MZX Tech LLC, the xAI/SpaceX subsidiary) is the "third building" Musk tweeted about, but it rolls up under Colossus II. They are **not breaking ground on a new "Colossus 3" campus**; the path to Musk's "almost 2 GW" runs through expanding the existing Colossus II footprint plus the stated next-phase GB300 expansion. No fourth/new campus has been announced as of 2026-06-22.

- Mississippi permitted **41 natural-gas turbines** for the site (since challenged in court by the NAACP). State pegged the investment at **$20B+**, the largest in its history. First-phase ops targeted Feb 2026.

### Reality-check on capacity `[HIGH]`

- The S-1 says Colossus + Colossus II *"collectively provide approximately 1.0 gigawatt"* installed as of filing, versus Musk's "almost 2 GW" target.
- Independent satellite analysis (Epoch AI via Tom's Hardware, Jan 2026) put Colossus 2's actual installed **cooling at only ~350 MW**, well below advertised 1 GW. As with GPU counts, announced runs well ahead of operational.

See [SOURCES.md](SOURCES.md) for full citations.
