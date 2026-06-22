# 06 · Grok & the AI product line (facts)

The AI segment is what Colossus exists to train. This is the product side; [03-ai-compute.md](03-ai-compute.md) is the infrastructure side.

## The model roadmap `[HIGH] on the tweet, [MED] on status`

Musk, **April 8, 2026** (X, 28.3M views), verbatim:

> "SpaceXAI Colossus 2 now has 7 models in training: Imagine V2, 2 variants of 1T, 2 variants of 1.5T, **6T**, **10T**. Some catching up to do."

So the 6-trillion and 10-trillion parameter models are real, and were **in training, not shipped**, as of April. Status as of 2026-06-22:

- **Current shipping flagship:** Grok 4.x (~**Grok 4.3**, shipped ~Apr 30, 2026), 1M-token context, native video input. `[MED]`
- **Grok 5 (the 6T model):** still in training on Colossus 2, **not released**. Targets slipped repeatedly (late 2025 → Q1 → Q2 2026), full API access now pointed at Q3. Prediction markets put **~45% odds it ships before September 2026** (Manifold), so a "frontier by September" outcome is an aggressive case, not a base case. `[MED]`
- **10T model:** pure aspiration, still pre-training, no release window. The "beat Anthropic" moonshot, est. ~$1.5B+ training cost. `[LOW]`
- **V9-Medium:** a separate **1.5T coding-focused model** trained on Cursor developer-workflow data, shipped ~**June 16, 2026** in consumer Grok and SuperGrok (API not yet open). This ties to the Cursor acquisition. `[MED]`
- **Benchmark standing (the gap to close):** Grok 4.3 scores **53 on the Artificial Analysis Intelligence Index, 4th place**, behind **Claude Opus 4.8 (61.4)**, GPT-5.5 (60.2), and Gemini 3.1 Pro (57). So xAI is **frontier-adjacent but not at the frontier**; the 6T/10T parameter bet is the attempt to close that ~8-point gap on Colossus 2. No independent Grok 5 / V9-Medium numbers exist yet. `[MED]`

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
