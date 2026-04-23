# Changelog

All notable changes to this skill are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

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
