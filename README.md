# foresight

**Professional multi-school futurist assistant for Claude.**

Responds in 🇫🇷 French · 🇬🇧 English · 🇪🇸 Spanish · 🇸🇦 Arabic based on the user's language.

---

## What it does

This skill turns Claude into a high-level foresight practitioner fluent in multiple
intellectual traditions. It selects the right method for the right horizon, names
its methodological choices, and always ends with concrete decision implications.

## Schools covered

| School | Key methods |
|---|---|
| 🇫🇷 French / LIPSOR (Godet) | MICMAC, MACTOR, SMIC, Morphological analysis |
| 🕊️ Humanist (Berger / de Jouvenel) | Futuribles, normative foresight, Jouvenel triptych |
| 🐚 Anglo-Saxon strategic | Shell Scenarios, Three Horizons, Cone of Plausibility, Backcasting |
| 🔍 Critical (Inayatullah) | Causal Layered Analysis (CLA) — 4 levels |
| 🌐 Institutional (NIC) | Global Trends methodology (≥15yr horizon) |
| 🔮 Anticipation (Poli) | Futures literacy, implicit vs. explicit anticipation |
| 🎯 Transversal | STEEP, PESTEL, Delphi, Futures Wheel, Wild cards, Schwartz axes |

## Key design decisions

- **Method-horizon matrix** — prevents methodological misuse (e.g. NIC on a 6-year horizon)
- **Probabilistic language** — calibrated as: certain / probable / possible / speculative / wild card
- **Jouvenel triptych** — possible / probable / souhaitable always distinguished
- **4 work modes** — Quick response, Full analysis, Facilitation, Deliverable
- **Deliverable specs** — each output type has structure + indicative page count

## File structure

```
foresight/
├── SKILL.md                          ← main skill (273 lines)
├── README.md                         ← this file
├── CHANGELOG.md                      ← version history
└── references/                       ← loaded on demand
    ├── godet-lipsor.md               ← MICMAC, MACTOR, SMIC, morphological
    ├── nic-global-trends.md          ← GT structure, GT2040 scenarios
    ├── cla-guide.md                  ← CLA step-by-step + examples
    ├── delphi-protocol.md            ← Delphi protocol + variants
    └── anglosaxon-tools.md           ← Cone of Plausibility, 3H, EIA, Wind Tunneling
```

## Trigger phrases (sample)

**FR:** "quels futurs possibles", "analyse prospective", "signaux faibles", "horizon 2030"
**EN:** "scenario planning", "weak signals", "strategic foresight", "futures studies"
**ES:** "prospectiva", "escenarios futuros", "señales débiles", "análisis de tendencias"
**AR:** "استشراف المستقبل", "سيناريوهات", "إشارات ضعيفة"

## Background

Built for a CNAM-trained futurist (Master 2010). Designed to be school-agnostic
and methodologically rigorous — not locked into any single tradition.

---

*Maintained with [Claude Skill Builder](https://claude.ai)*
