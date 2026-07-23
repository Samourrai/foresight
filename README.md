# Changelog

All notable changes to this skill are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [2.3.0] — 2026-07-20

### Fixed
- **Corrected ADDIS Drafting-phase step name**: "Consult" → **"Review"**, matching the
  canonical Decision Thinking Template (ADDIS v5.3, Innovation for Policy Foundation, 2024)
  supplied directly by the user. The website overview text uses "Consult" for the same
  definition; the downloadable template — the authoritative source — uses "Review." Both
  terms are now documented, with Review as primary.
- Fixed in: `references/addis-methodology.md` (steps table, method bridge table,
  participatory principles, canvas) and `SKILL.md` (ADDIS school step sequence,
  Mode ADDIS Overlay bridge and principles).

### Added
- **Template Header Fields** section in `references/addis-methodology.md`: the 4 framing
  fields from the official template (Policy Vision, Policy Goal, Who is Concerned?,
  Decision Instrument) that precede the 12-step canvas — previously missing entirely.
- Replaced the invented ASCII canvas with an **"ADDIS Canvas — Official Template Layout"**
  section that reproduces the real template structure (header fields + 12-step table),
  sourced directly from the official PDF.
- Source citation updated to the specific template version (v5.3, 2024, CC BY-SA 4.0,
  community@i4policy.org).

---

## [2.2.0] — 2026-07-20

### Changed
- **Replaced silent language auto-detection with an explicit upfront choice.**
  On first activation in a conversation, the skill now asks the user to select a
  working language (🇫🇷/🇬🇧/🇪🇸/🇸🇦) via `ask_user_input_v0` before starting any
  analysis, instead of guessing from message content. The choice persists for the
  rest of the conversation — asked once, not on every message.
- New "Étape 0 — Choix de la langue" section at the top of SKILL.md replaces the
  old "Tu détectes la langue..." posture bullet.
- Tightened the intro/voice-setting paragraph for brevity.

### Rationale
Auto-detection was a silent guess that could misfire on short or ambiguous first
messages (e.g. a pasted URL, a name, a number). An explicit one-time choice is more
reliable, costs one extra turn only at the very start, and removes ambiguity for
the rest of the engagement — net efficiency gain despite the small size increase.

---

## [2.1.0] — 2026-07-20

### Changed — Efficiency Pass
- **Extracted multilingual terminology table** (20 concepts × 4 languages, 31 lines) from
  SKILL.md into new `references/multilingual-terms.md` (35 lines) — loaded on demand only
  for EN/ES/AR responses or term translation, instead of always occupying context
- **Added Quick Mode Selector** at the top of "Flux de travail" — a 6-row lookup table
  mapping request signals to work modes, so mode routing no longer requires reading all
  5 mode blocks in full
- **Tightened Mode Program Design and Mode ADDIS Overlay** — merged the repeated
  "Load `references/X.md` immediately" sentence into a compact 🔽 marker on the heading;
  condensed numbered steps to single lines where possible
- **Result**: SKILL.md reduced from 19,791 to 17,721 characters (~10.5% smaller
  always-loaded footprint), 334 → 316 lines, with zero loss of routing accuracy or
  methodological content — everything removed from the main file is preserved verbatim
  in reference files

### Added
- New reference file: `references/multilingual-terms.md`

---

## [2.0.0] — 2026-07-20

### Added
- **ADDIS Decision Thinking methodology** (`references/addis-methodology.md`, 175 lines)
  - Source: i4Policy / decisionthinking.org — 5 phases, 12 steps
    (Agenda Setting: Care/Initiate/Define; Drafting: Ideate/Develop/Consult;
    Decision-Making: Propose/Adopt; Implementation: Deliver/Monitor;
    Sense-Making: Harvest/Understand)
  - Foresight-ADDIS method bridge table: maps each ADDIS step to the foresight
    method that feeds it (scenarios → Ideate, backcasting → Develop,
    Wind Tunneling → Propose, Early Warning System → Monitor, etc.)
  - "When to use ADDIS overlay" decision table (public policy: yes;
    single-decision-maker corporate strategy: optional)
  - 5 participatory design principles (Care before Define, Consult must
    visibly change the draft, Adopt needs legitimate process, Monitor
    pre-committed at Adopt, Harvest mandatory)
  - ADDIS Canvas quick-reference template (12-cell guiding questions)
- New school section in SKILL.md: **Decision Thinking — ADDIS (i4Policy)**
- New work mode: **Mode ADDIS Overlay** — for engagements that must end in
  an adopted institutional decision, not just a report
- New quality standard #9: **Légitimité décisionnelle** — apply ADDIS overlay
  when the deliverable must be an adopted decision, not just a forecast
- New recommended combination: `Foresight (scénarios/backcasting) + ADDIS`
- ADDIS terms added to multilingual terminology table (décision adoptée,
  co-création citoyenne)
- Trigger keywords added: "ADDIS", "decision thinking", "policy co-creation",
  "agenda setting"

### Changed
- Reference table updated with `addis-methodology.md` entry
- Description trimmed and reorganized to fit new keywords within 1024 char limit

---

## [1.2.0] — 2026-04-23

### Added
- **Consulting program design capability** (`references/consulting-program.md`, 424 lines)
  - Phase 0: Client brief template (12 scoping questions), Study Design Document template
  - Phase 1: Environmental scan — source typology, signal classification grid,
    expert panel design (composition, recruitment, interview guide)
  - Phase 2: Structural analysis — tool selection guide, MICMAC/MACTOR workflow
  - Phase 3: Scenario construction — architecture selection, 9-element narrative template,
    validation workshop protocol
  - Phase 4: Strategic implications — Wind Tunneling robustness matrix, Backcasting,
    Early Warning System design
  - Phase 5: Communication — deliverable stack by audience, 15-slide executive
    presentation structure, knowledge transfer protocol
  - Program governance: meeting cadence, QA process, 5-risk register
  - Three timeline templates: compact / standard / comprehensive
- **Mode: Program Design** added as 5th work mode in SKILL.md
- Consulting-specific trigger phrases added to description

---

## [1.1.0] — 2026-04-23

### Added
- **Multilingual support (FR/EN/ES/AR)**
  - Trigger keywords in English, Spanish, and Arabic added to description
  - Automatic language detection: responds in the user's language
  - Arabic: formal register (الفصحى) enforced
  - Multilingual terminology table: 18 key foresight concepts × 4 languages
  - Note on Arabic academic usage of technical method names (MICMAC, CLA, etc.)
- Title updated to display all 4 languages

### Changed
- Posture rule: "default French" replaced by automatic language detection

---

## [1.0.0] — 2026-04-23

### Added
- **Core skill** (`SKILL.md`, 238 lines)
  - 7 foresight schools: French/LIPSOR, Humanist, Anglo-Saxon, Critical/CLA,
    NIC/Global Trends, Anticipation/Poli, and transversal methods
  - Method-horizon selection matrix (short/medium/long/very long × context)
  - ⚠️ Critical rule: NIC/Global Trends restricted to horizons ≥15 years
  - Cone of Plausibility (Voros) as universal framing tool
  - Jouvenel triptych formalized (possible / probable / souhaitable)
  - Emerging Issues Analysis (Molitor) with maturity curve
  - STEEP alongside extended PESTEL
  - 4 work modes: Quick response / Full analysis / Facilitation / Deliverable
  - Deliverable format specs with page counts
  - Probabilistic language calibration (certain / probable / possible / speculative / wild card)
  - 5 recommended method combinations
  - 7 quality standards including horizon/method coherence rule

- **Reference files** (loaded on demand)
  - `references/godet-lipsor.md` — MICMAC, MACTOR, SMIC, morphological analysis
  - `references/nic-global-trends.md` — GT structure, GT2040 scenarios, sector adaptation
  - `references/cla-guide.md` — CLA step-by-step, city example, workshop usage
  - `references/delphi-protocol.md` — Classic protocol, variants, Delphi+SMIC integration
  - `references/anglosaxon-tools.md` — Cone of Plausibility, Three Horizons,
    Emerging Issues Analysis, Wind Tunneling
