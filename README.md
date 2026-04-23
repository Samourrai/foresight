# foresight

**Professional multi-school futurist assistant for Claude.**

Responds in 🇫🇷 French · 🇬🇧 English · 🇪🇸 Spanish · 🇸🇦 Arabic based on the user's language.

------
## Who Does it
Issam Ourrai is a Product Owner in financial markets software, doctoral researcher in entrepreneurial ecosystems, and lecturer in digital innovation and data science at IÉSEG School of Management and ISC Paris. He is the founder of Creativebox.ma, an incubator and coworking space in Morocco, and an active builder at the intersection of AI, law, and entrepreneurship.
His sports law skill was developed out of a practical need observed across African and European football clubs: the gap between regulatory complexity and operational decision-making on the ground. Drawing on his research background in institutional frameworks and his experience building AI-powered tools for non-technical users, he designed this skill so that a club manager facing a CAF notice at 11pm gets a usable answer — not a textbook.
Based in Paris. Research interests: entrepreneurial ecosystems, frugal innovation, informal economies, and AI applications for practitioners.
🌐 ourrai.net · 📍 Paris, France

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
    ├── anglosaxon-tools.md           ← Cone of Plausibility, 3H, EIA, Wind Tunneling
    └── consulting-program.md         ← Full 5-phase consulting engagement guide
```

## Trigger phrases (sample)

**FR:** "quels futurs possibles", "analyse prospective", "signaux faibles", "horizon 2030"
**EN:** "scenario planning", "weak signals", "strategic foresight", "futures studies"
**ES:** "prospectiva", "escenarios futuros", "señales débiles", "análisis de tendencias"
**AR:** "استشراف المستقبل", "سيناريوهات", "إشارات ضعيفة"

## Consulting program capability

The skill can design and manage a full foresight research program for consulting engagements:

| Phase | Content |
|---|---|
| **0 — Scoping** | Client brief (12 questions), study design document |
| **1 — Environmental scan** | Source typology, signal grid, expert panel design, interview guide |
| **2 — Structural analysis** | MICMAC/MACTOR selection and workflow |
| **3 — Scenarios** | Architecture selection, narrative template, validation workshop |
| **4 — Strategic implications** | Wind Tunneling matrix, Backcasting, early warning system |
| **5 — Communication** | Deliverable stack by audience, 15-slide exec deck structure |

Timeline templates: compact (6–8 wks) / standard (3–4 mo) / comprehensive (6–12 mo)

## Background

Built By a CNAM-trained futurist (Master 2010). Designed to be school-agnostic
and methodologically rigorous — not locked into any single tradition.

---

*Maintained with [Claude Skill Builder](https://claude.ai)*
