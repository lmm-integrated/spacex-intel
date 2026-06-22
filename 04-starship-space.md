# 04 · Starship & space-based AI

## Starship Flight 13: has NOT flown `[HIGH]`

As of 2026-06-22, **Flight 13 has not launched.** It is in pre-flight integration at Starbase and grounded pending FAA approval of the Flight 12 mishap investigation.

Hardware status (X @LunarCitizens, Jun 22):
- **Ship 40:** engines installed Jun 19, static fire imminent.
- **Booster 20:** cryo test completed Jun 10, engine installation underway, "33 Raptors expected in ~5 weeks."
- Both are Starship **Version 3 / Raptor 3**.

SpaceX filed an FCC request for higher-power comms for an **"Orbital Return Demo" mission**, window **July 29 to December 28, 2026** (X @muskonomy, Jun 21), consistent with a NET late-July/August target. No tower catch is planned for Flight 13; a catch is contemplated only for **Flight 14+** after two clean soft splashdowns. Flight 14 is teased as potentially the first V3 booster catch, first orbital insertion, first operational Starlink deployment, and first ship catch.

## Flight 12 (the one that actually flew) `[HIGH]`

Launched **2026-05-22, 22:30 UTC** from Pad 2, Starbase, the **V3 / Raptor 3 debut**.
- **Ship S39 succeeded:** deployed ~22 Starlink simulators, survived reentry, controlled soft splashdown in the Indian Ocean.
- **Booster B19 failed:** most of its 33 engines failed to relight on the boostback burn; crashed into the Gulf at ~1,450 km/h. This triggered the FAA grounding.

If you've seen a description of "Flight 13" with a V3 debut, booster splashdown failure, and Starlink simulators, that's actually Flight 12.

## Core space business context `[MED]`

- **Launch cadence:** record ~165 orbital launches in 2025; pacing toward ~140-145 Falcon launches in 2026. Swept 100% of NSSL Phase 3 Lane 1 task orders. ~$22B cumulative federal awards.
- **Starlink:** 12M+ subscribers, $11.4B 2025 revenue at ~63% EBITDA margin, ~$15.5B run-rate for 2026; $17B EchoStar spectrum deal (Sept 2025) underpins Direct-to-Cell.
- **Artemis:** NASA resequenced (Feb 2026). Artemis III is now a crewed LEO demo (~late 2027); first crewed lunar landing slips to Artemis IV (~2028).

## AI1: the orbital data-center satellite `[HIGH] unveiled, [LOW] feasibility`

Officially unveiled **2026-06-08** by SpaceX (official @SpaceX post + @SawyerMerritt specs), days before the IPO, at spacexipo.com.

- **150 kW peak compute** (120 kW average), **70 kW per ton**, **compute provider interchangeable** (not locked to one chipmaker).
- **~70 m wingspan** (wider than a Boeing 747-8), ~20 m tall deployed; solar at 250 W/m², liquid-radiator cooling.
- Reuses Starlink V3 bus tech; launches on Starship.
- **Target: 1 GW of orbital AI compute by late 2027** from a new **11M-sq-ft "Gigasat" factory in Bastrop County, TX** (~1,000 acres). That would require launching ~6,000+ AI1 satellites per year.

**Status: a design.** First prototypes target early 2027; nothing is in orbit. The Anthropic/Google billions are for the **terrestrial** Colossus, not AI1 (frequent conflation). Economics, thermal management, and the launch cadence are unproven and very aggressive.

### For comparison (not SpaceX)
- **Starcloud-1** (Nvidia H100, launched Nov 2, 2025 on a Falcon 9) did the first in-orbit LLM inference and training, the only space-AI effort to fly working hardware so far. Independent startup, not Musk.
- **Google Project Suncatcher** (orbital TPUs with Planet) is also pre-prototype, ~2027.

See [SOURCES.md](SOURCES.md) for full citations.
