# Wiki Log

Append-only chronological record of all activity: ingests, queries, and lint passes.

To view recent activity: `grep "^## \[" log.md | tail -10`

---

## [2026-04-07] init | Wiki created

Wiki initialised for a technical writer's personal knowledge base.

Structure created:
- `raw/` — source documents folder
- `wiki/` — LLM-maintained knowledge base
- `wiki/sources/` — per-source summary pages
- `CLAUDE.md` — schema and operating instructions

Core pages created:
- `wiki/index.md`
- `wiki/log.md`
- `wiki/overview.md`
- `wiki/glossary.md`

Next step: Drop your first source into `raw/` and say **"ingest [filename]"**.

---

## [2026-05-22] ingest | Full raw/ batch (4 PDFs)

**Sources ingested:**
- `Agency_lit_review-HAL.pdf` — Voysey et al., child–AI agency rapid review
- `3544548.3580651.pdf` — Bennett et al., CHI 2023 HCI agency/autonomy review
- `3628516.3655806.pdf` — Iivari et al., IDC 2024 transformative agency
- `1-s2.0-S2212868923000545-main.pdf` — IJCCI computational empowerment editorial

**Pages created:**
- Sources: `agency-lit-review-hal`, `bennett-chi23-hci-agency-autonomy`, `iivari-idc24-transformative-agency`, `ijcci-computational-empowerment-editorial`
- Concepts: `agency`, `autonomy`, `child-ai-interaction`, `computational-empowerment`, `transformative-agency`, `relational-agency-lens`, `hci-agency-autonomy-four-aspects`
- Personas: `children-digital-users`
- Analyses: `agency-research-landscape`

**Pages updated:** `index`, `overview`, `glossary`, `log`

**Key additions:**
- Canonical agency definition and three child–AI agency forms (self / system / environment)
- Bennett four-aspects framework for general HCI
- Computational Empowerment + transformative agency as CE fourth component
- Relational agency lens for multi-stakeholder design
- Glossary terms and style conventions for agency-related writing

---

## [2026-05-22] lint | English (GB) normalisation

**Issues found:** US spellings and locale inconsistencies (`toward`, `artifact`, `catalog`, `capitalization`, `initialized`, `Criticizing`, `Analytic`); index assistant-facing wording.

**Fixes applied:**
- Normalised spelling across all wiki pages to en-GB
- Added [[english-gb]] style rule; updated [[glossary]] and [[index]]
- Revised index introduction to reader-facing catalogue wording

---

## [2026-05-22] maintain | Bibliography

**Pages created:** `bibliography.md`

**Pages updated:** `index`, `overview`, all four `wiki/sources/*` pages, `CLAUDE.md`

**Key additions:**
- Master bibliography (Harvard author–date + BibTeX) for four ingested papers
- Cite keys (`Voysey2026`, `Bennett2023`, `Iivari2024`, `Schaper2023`) linked from source pages
- Ingest workflow now requires bibliography update on every new `raw/` document
