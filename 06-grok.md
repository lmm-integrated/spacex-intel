# 06 · Grok & the AI product line (facts)

The AI segment is what Colossus exists to train. This is the product side; [03-ai-compute.md](03-ai-compute.md) is the infrastructure side.

## The model roadmap `[HIGH] on the tweet, [MED] on status`

Musk, **April 8, 2026** (X, 28.3M views), verbatim:

> "SpaceXAI Colossus 2 now has 7 models in training: Imagine V2, 2 variants of 1T, 2 variants of 1.5T, **6T**, **10T**. Some catching up to do."

So the 6-trillion and 10-trillion parameter models are real, and were **in training, not shipped**, as of April. Status as of 2026-06-22:

- **Current shipping flagship:** Grok 4.x (~**Grok 4.3**, shipped ~Apr 30, 2026), 1M-token context, native video input. `[MED]`
- **Grok 5 (the 6T model):** still in training on Colossus 2, **not released**. Targets slipped repeatedly (late 2025 → Q1 → Q2 2026). `[HIGH on "not shipped"]`
- **10T model:** pure aspiration, still pre-training, no release window. The "beat Anthropic" moonshot, est. ~$1.5B+ training cost. `[LOW]`
- **V9-Medium:** a separate **1.5T coding-focused model** trained on Cursor developer-workflow data, shipped ~**June 16, 2026** in consumer Grok and SuperGrok (API not yet open). This ties to the Cursor acquisition. `[MED]`
- **Benchmarks:** no independent Grok 5 / V9-Medium numbers yet. For reference, Grok 4 trailed the frontier on coding (SWE-bench ~75% vs Claude Opus 4.7 at 87.6%). Grok is currently **behind** Claude/GPT on coding. `[MED]`

"Some catching up to do" is Musk's own framing, and it's accurate: the parameter-count race is a bet that scale on Colossus 2 closes a real current quality gap.

## Usage & monetization (from the S-1) `[HIGH]`

- **117M MAU** for Grok AI features (March 2026), out of **~550M combined Grok + X MAU** (so ~20% of the ecosystem touches Grok AI).
- **xAI FY2025:** $3.2B revenue, **$6.4B operating loss** (vs 2024: $2.62B rev, $1.56B loss). Spending is accelerating, not slowing.
- 2025 revenue mix: ~$365M X/Grok subscriptions + ~$88M data licensing + ~$116M advertising.
- Pricing: SuperGrok ~$30/mo, SuperGrok Heavy ~$300/mo, plus usage-based API.
- Standalone Grok revenue ~$500M in 2025, projected ~$2B in 2026 `[LOW: secondary estimate, not in S-1]`.

## Training compute `[MED-HIGH]`

- Trains on **Colossus 2** (~1 GW, ~550,000 GB200/GB300 GPUs, ~$18B hardware). See [03-ai-compute.md](03-ai-compute.md) for the cluster detail.
- **AI-segment capex: $12.7B (2025) rising to ~$7.7B in Q1 2026 alone** (~$30B annualized run-rate). This is the cash furnace the IPO and bond are feeding.

## Why it matters

Grok/xAI is the loss-making, capital-hungry leg, but it's also the reason for the orbital-datacenter narrative and the compute-leasing business. The investment question (see [08-forward-thesis-valuation.md](08-forward-thesis-valuation.md)) largely turns on whether this segment becomes a frontier-model winner or stays a ~$6B/yr loss leader that mainly exists to fill (and justify) Colossus.

See [SOURCES.md](SOURCES.md) for citations.
