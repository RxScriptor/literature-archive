---
slug: qin-nodate-advanced-science-dc-targeting-pls2
title: "A Nanobody-LNP Platform for Targeting and Relicensing Dendritic Cells for Potent Cancer Immunotherapy"
first_author: "Shugang Qin"
last_author: "Xiangrong Song"
journal: "Advanced Science"
journal_abbr: null
year: null
doi: 10.1002/advs.202523024
url: https://onlinelibrary.wiley.com/doi/abs/10.1002/advs.202523024
zotero_key: EWGGB2KN
category: "LNP"
keep_tag: keep/LNP
generated_at: 2026-05-06
---

# A Nanobody-LNP Platform for Targeting and Relicensing Dendritic Cells for Potent Cancer Immunotherapy

> Shugang Qin et al. (, Advanced Science)  
> DOI: [10.1002/advs.202523024](https://doi.org/10.1002/advs.202523024) · Zotero: [`EWGGB2KN`](zotero://select/items/EWGGB2KN)

## 1. TL;DR

DC2.1 nanobody로 표면 수식한 LNP가 dendritic cell (DC) 표면 단백질 PLS2 (Plastin-2)에 결합 → 93% DC 내재화. 같은 결합이 Leptin–JAK2–STAT3 면역억제 경로를 동시에 downregulate해 DC 성숙을 함께 유도. E.G7-OVA 마우스 lymphoma 모델에서 antigen-specific CD8+ T cell 3–4× 확장과 거의 완전한 종양 퇴축. PLS2를 DC delivery + immunomodulation 동시 표적으로 새롭게 제시.

## 2. Background & motivation

현재 mRNA cancer vaccine은 임상 ORR (objective response rate)이 낮음. 일부는 LNP biodistribution이 DC-rich 조직에 효율적으로 도달하지 못하고, 일부는 tumor microenvironment에서 DC가 immunosuppressive 상태로 잡혀있기 때문. 기존 active targeting 전략 (carbohydrate, peptide, antibody, nanobody)은 대체로 antigen 전달 효율 향상에 머물고 DC 자체의 maturation checkpoint는 건드리지 않음.

이 논문은 nanobody-conjugated LNP가 단일 ligand로 (1) DC-preferential delivery + (2) DC maturation re-licensing을 **동시에** 달성할 수 있는지 묻고, PLS2 표적이 leptin–JAK2–STAT3 axis를 차단해 양쪽 효과를 만들어낸다는 결과를 제시.

## 3. Key findings

- **Conjugate**: DC2.1–PEG2k–Chol을 maleimide-thiol로 합성, 92% coupling efficiency, 9일 안정. PLS2에 Kd = 5.46 × 10⁻⁹ M (high-affinity binding).
- **LNP composition**: IC2 (ionizable) / DOPE / Chol / DMG-PEG2k = 35 : 16 : 46.5 : 2.5 molar, microfluidic mixing, 직경 ~160 nm, ZP −3 mV, mRNA encapsulation > 90%. SM-102 / ALC-0315 등 임상 ionizable lipid는 아니라 transferability 별도 검증 필요.
- **Selectivity**: DC2.4 (DC line) 93.27% binding > RAW264.7 (macrophage) 65.03% > A549 (lung epithelial) 36.32% — phagocyte 우선이지만 DC 우선. Cellular uptake은 CPZ로 차단되는 clathrin-mediated endocytosis. 마우스 SC 투여 후 IVIS biodistribution에서 spleen DC, dLN cDC1/cDC2 모두 LNP / MNP 대조군 대비 유의 enrichment.
- **Mechanism**: Nb-LNP 처리 DC의 transcriptomics에서 Lep / JAK2 / STAT3 cluster 유의 downregulation, qRT-PCR로 검증. AlphaFold 예측 (pTM > 0.8) + 100 ns MD simulation으로 DC2.1–PLS2 complex의 구조적 안정성 입증 (in silico only — X-ray / cryo-EM 미수행). Protein corona 분석에서 Nb-LNP는 immunoglobulin + C1qc enrichment + fibrinogen↑로 complement-priming 환경 형성.
- **Efficacy in vivo**: E.G7-OVA syngeneic lymphoma (C57BL/6, n=5) IV 3회 dose → OVA-specific tetramer+ CD8+ T cell이 LNP / MNP 대조군 대비 3–4× 확장 (p < 0.05 vs all controls), 일부 마우스 거의 완전한 종양 퇴축. NPC LMP2 model (n=6)에서 동일 트렌드 (p = 0.0159 vs MNP@LMP2).
- **Safety**: ALT, AST, CRE, urea, total protein, LDH 모두 정상. H&E (heart / liver / spleen / lung / kidney) 병리소견 없음.

## 4. Implication for our LNP work

PLS2 표적은 두 측면에서 새로운 design lever를 시사. (1) DEC-205 / CLEC9A 같은 기존 DC-targeting receptor의 대안으로, nanobody scaffold는 antibody 대비 GMP scale 친화적이고 conjugation 전략 (DMG-PEG2k 일부를 nanobody-PEG-Chol로 치환)이 기존 LNP 제조 워크플로에 직접 끼워넣을 수 있음. (2) 단순 표적화가 아니라 **수용체 결합 자체로 immunosuppressive checkpoint를 동시 차단**하는 컨셉 — antigen 전달 + DC re-licensing이 한 ligand로 묶이는 dual-action design. 차세대 mRNA 백신 LNP에서 "delivery × immunomodulation co-targeting" 패턴 후보로 추적할 가치가 있음.

한계도 분명함. PLS2는 macrophage / neutrophil 등 phagocyte 일반에 발현 (RAW264.7 65% binding) — cDC1 / cDC2-specific은 아님. 본 연구는 IC2 ionizable lipid 기반이라 SM-102 / ALC-0315 등 다른 lipid backbone에서 nanobody-PEG-Chol 치환이 동일한 결과를 줄지 별도 검증 필요. 임상 translatability 평가에는 humanized PLS2 binding profile + nanobody immunogenicity (ADA risk) 데이터가 우선.

## 5. Limitations / open questions

- 모든 in vivo는 마우스 syngeneic tumor (E.G7-OVA lymphoma, NPC-LMP2 derivative). 인간 DC subset 분포 및 PLS2 발현 프로파일은 마우스와 다를 수 있어 translation 미검증.
- PLS2가 macrophage / neutrophil에도 발현 — DC-specific이 아닌 phagocyte 광범위 표적. Long-term off-target macrophage 효과 (TAM 재극화 등) 미평가.
- DC2.1–PLS2 binding interface는 AlphaFold + MD 예측만 — 실측 high-resolution structure (X-ray / cryo-EM) 없음. Nanobody developability (humanization, ADA, half-life) 미수행.
- Lep–JAK2–STAT3 downregulation 기전은 actin remodeling 또는 LepR signaling steric hindrance 가설 — 분자기전 직접 입증 없음 (transcriptomic correlation level).
- N = 4–6 (tumor experiments), N = 3 (biodistribution) — 통계 power 보통, 독립 코호트 replication 없음.
- 3회 IV regimen만 검증 — dose-response, repeat-dosing tolerance, immune memory durability 미평가.
- DEC-205 antibody-conjugate, CD40L LNP 등 기존 DC-targeting 전략과 직접 head-to-head 비교 없음.

---

<details>
<summary>Abstract (raw)</summary>

Effective cancer immunotherapy requires not only efficient antigen delivery to dendritic cells (DCs) but also overcoming local immunosuppression. Here, we introduce a nanobody-LNP platform that achieves both targeting and active relicensing of DCs. By decorating lipid nanoparticles with nanobodies against the DC surface protein Plastin-2 (PLS2), our platform achieves a remarkable 93% internalization efficiency. This preferential targeting dramatically enhances antigen expression while simultaneously relicensing DCs toward a more potent, mature phenotype by inhibiting the immunosuppressive Leptin-JAK2-STAT3 signaling pathway. This integrated strategy unleashed potent cytotoxic T lymphocyte responses and led to marked inhibition of established tumors. Our work establishes PLS2 as a novel immunomodulatory receptor and presents a dual-action delivery platform that significantly boosts cancer vaccine potency.

</details>
