---
title: "Personalized Child Speech Recognition via Test-Time Adaptation (Shi et al., 2024)"
type: source
created: 2026-05-22
updated: 2026-05-22
sources: [Shi2024_Personalized-Speech-Recognition-for-Chil.pdf]
tags: [speech-recognition, test-time-adaptation, child-AI, accessibility]
---

# Personalized Child Speech Recognition

Test-time adaptation (SUTA, SGEM) for off-the-shelf ASR on per-child speech variability in child–AI and social robot interaction.

---

## Metadata

| Field | Value |
|---|---|
| Authors | Zhonghao Shi, Xuan Shi, Anfeng Xu, Tiantian Feng, Harshvardhan Srivastava, Shrikanth Narayanan, Maja Matarić |
| Year | 2024 |
| Venue | Speech/ASR conference paper |
| Raw | `Shi2024_Personalized-Speech-Recognition-for-Chil.pdf` |
| Cite key | `Shi2024` — [[bibliography]] |

---

## Key findings

- Off-the-shelf ASR poorly generalises to children's acoustic/linguistic variability (domain shift from adult pre-training)
- Training-time adaptation limited in deployment: needs labelled child data, cannot adapt per new child at runtime
- **Test-time adaptation** improves both average and per-child performance vs unadapted baselines
- TTA still struggles with **non-linguistic** child speech
- Enables continuous unsupervised personalisation for conversational child-facing agents and socially assistive robots

---

## Relevance to child–AI interaction

Infrastructure for equitable voice interaction: without per-child ASR, children's **agency** in dialogue (commands, storytelling, tutoring) is constrained by recognition failure.

---

## Related pages

- [[child-ai-interaction]]
- [[children-digital-users]]
- [[bibliography]]
