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

---

## [2026-05-22] ingest | papers.bib batch (24 PDFs, 5×5)

**Source:** `D:\Agency\papers.bib` (62 entries) — 24 open-access PDFs downloaded to `D:\Agency\sources\`, copied to `raw/`

**Setup:**
- Download scripts: `download_papers.py`, `download_papers_pass2.py`
- Pending list: `D:\Agency\sources\papers-to-download.md` (38 not obtained)
- Ingest batches: 5 papers per batch with topic review in [[ingest-batches-child-ai-topics]]

**Pages created (26):**
- Sources (24): `bai-2023-participatory-design-ai-children`, `bennetot-2020-help-seeking-hri`, `chowdhury-2023-goldilocks-child-centered-ai`, `choi-2026-tinker-tales`, `chubb-2021-ethical-conversational-ai-children`, `druga-2025-scratch-copilot`, `dwivedi-2023-values-ai-problem-formulation`, `figueiredo-2025-conversational-agents-kids`, `fors-2022-children-centric-ai-growth`, `hoehl-2024-honest-machines-trust`, `kim-2025-young-children-anthropomorphism-ai-chatbot`, `lee-2022-interactive-children-story-rewriting`, `lemaignan-2016-learning-by-teaching-robot-handwriting`, `lemaignan-2021-unicef-guidance-ai-children-robot`, `nanduri-2023-revitalizing-endangered-languages-ai`, `neugnot-cerioli-2024-future-child-development-ai`, `ragone-2024-designing-safe-engaging-ai-experiences`, `rudenko-2024-child-factor-child-robot-interaction`, `shi-2024-personalized-speech-recognition-children`, `sun-2024-parent-needs-preschoolers-storytelling`, `xie-2024-evaluation-scheme-children-centered-language`, `yang-2025-autiverse-autistic-adolescents-journaling`, `yang-2026-design-framework-children-agency`, `yatani-2024-ai-extraherics-higher-order-thinking`
- Meta: `papers-pending-download`, `ingest-batches-child-ai-topics`

**Pages updated:** `index`, `overview`, `glossary`, `bibliography`, `child-ai-interaction`, `log`

**Bibliography:** 28 cite keys in summary table (4 agency + 24 papers.bib); compact Harvard entries added for papers.bib batch

**Batch topic reviews ([[ingest-batches-child-ai-topics]]):**
1. PD, help-seeking, recommenders, co-creation, ethical CAI
2. Scratch Copilot agency, values in ML, CA scaffolds, growth model, trust
3. Anthropomorphism, story rewriting, teaching robots, UNICEF, language revitalisation
4. Child development + AI, UI/UX safety, CRI development, speech, parents/preschool
5. Evaluation rubrics, neurodiverse youth, agency PD framework, extraherics

**Key additions:** Co-creative (non-tutoring) child–AI; recommender/agency critique; parent-centred and trust themes; Yang & Zhao agency PD framework

---

## [2026-05-22] maintain | Index, bibliography, log sync

**Pages updated:** `index`, `bibliography`, `log`

**Key additions:** Full bibliography tables for all 28 ingested PDFs; log entry expanded with complete file list and cite keys
