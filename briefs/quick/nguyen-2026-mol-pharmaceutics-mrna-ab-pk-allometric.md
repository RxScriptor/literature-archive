---
slug: nguyen-2026-mol-pharmaceutics-mrna-ab-pk-allometric
title: "Application of Allometric Scaling and Translational Modeling to Predict Human Pharmacokinetics of mRNA-Encoded Antibodies"
first_author: "Tam N. T. Nguyen"
last_author: "Shu-Pei Wu"
journal: "Molecular Pharmaceutics"
journal_abbr: "Mol. Pharmaceutics"
year: 2026
doi: 10.1021/acs.molpharmaceut.5c01615
url: https://doi.org/10.1021/acs.molpharmaceut.5c01615
zotero_key: 95DADZHP
category: "LNP"
keep_tag: keep/LNP
generated_at: 2026-05-07
suitability: internal-only
---

> ⚠️ **internal-only**: competitor (BioNTech 직접 + Moderna 검증) 직결도 높음. **Public `literature-archive` repo에 commit 금지**. 검토 후 dds-work 또는 briefing-dashboard 같은 Private 위치로 이동 권장.

# Application of Allometric Scaling and Translational Modeling to Predict Human Pharmacokinetics of mRNA-Encoded Antibodies

> Tam N. T. Nguyen et al. (2026, Molecular Pharmaceutics)  
> DOI: [10.1021/acs.molpharmaceut.5c01615](https://doi.org/10.1021/acs.molpharmaceut.5c01615) · Zotero: [`95DADZHP`](zotero://select/items/95DADZHP)

## 1. TL;DR

mRNA-LNP에서 in vivo 발현되는 항체 (RiboMab platform)의 cross-species PK 예측 framework — 임상+전임상 두 분자 (BNT141/RiboMab01 IgG1, BNT142/RiboMab02.1 bispecific T-cell engager) 데이터로 allometric scaling 지수 도출, 외부 분자 (mRNA-1944/CHKV-24)로 검증. NHP single-species scaling이 인간 PK 1.33-fold 이내 예측. mRNA-encoded 항체 FIH dose 결정 가속화하는 platform 접근.

## 2. Background & motivation

mRNA-LNP 플랫폼은 단일 제조 공정으로 임의 단백질 in vivo 발현 가능 — 항체 후보 다수를 별도 cell line 없이 임상 평가 가능한 modular technology. 그러나 FIH dose 결정이 bottleneck. 소분자 / 일반 mAb / AAV gene therapy에는 allometric scaling이 정착됐지만 mRNA-LNP encoded protein은 인간 PK 데이터로 검증된 scaling 없었음 (기존 보고 3건 모두 인간 데이터 검증 부재).

본 연구는 두 임상 진행 분자 (NCT04683939 BNT141, NCT05262530 BNT142) 임상+전임상 PK + 외부 데이터 (mRNA-1944 NHP/healthy volunteer NCT03829384)를 활용해 platform allometric scaling + mechanistic translational model 두 framework을 인간 데이터로 직접 검증.

## 3. Key findings

- **Multi-species allometric exponents**: BNT141 DCmax exponent −1.29, DAUC −1.13; BNT142 DCmax −1.42, DAUC −1.38. 모두 음의 지수 — 큰 종일수록 dose-normalized exposure 감소. 두 매우 다른 분자 (전체 IgG1 vs bispecific Fab-scFv fragment)에서 일관된 패턴 → cross-platform generalizability.
- **Generalized single-species exponents**: 마우스 −1.26, NHP −0.75. NHP-from-1-species scaling으로 BNT141/142 DCmax/DAUC 인간 예측 모두 2-fold 이내. 마우스에서는 최대 4.44-fold 오차 (BNT141 DAUC). 외부 mRNA-1944 검증에서도 NHP-based 1.73-fold (DCmax) / 2.21-fold (DAUC) 이내.
- **Translational mechanistic model**: mRNA-LNP elimination (k_elim,mRNA) + translation rate (k_translate) + 2-compartment Ab disposition (CL_Ab, V1, V2, Q_Ab) 통합. translation rate scaling exponents −0.43 (RiboMab01), −0.59 (RiboMab02.1) — 큰 종일수록 translation efficiency 감소. CL_Ab exponent ~0.80 (전형적 mAb scaling exponent와 일치). NHP-from-NHP 단일 종 예측: BNT141/142 DCmax/DAUC 1.33-fold 이내 + concentration-time profile 충실 재현.
- **External validation (mRNA-1944 / Moderna CHKV-24)**: 다른 LNP formulation, NHP only 전임상 데이터로 인간 PK 예측 — 첫 56일 + 420일 long-term concentration-time profile 재현, DCmax/DAUC 1.52-fold 이내. 다른 mRNA backbone + 다른 LNP에서도 framework 일반화.
- **Translation efficiency 종간 격차**: 마우스 single-species 4-fold 오차는 ktranslate exponent −0.51로 species translation efficiency 차이 큼을 의미 (West et al. 2002 metabolic rate −0.25, mitochondrial transcript scaling −0.28~−0.4 패턴과 일치). 마우스 → 인간 extrapolation 정확도 한계의 mechanistic 근거.
- **임상 dose-equivalent 비교**: 마우스 IV에서 BNT141 10 μg ≈ 80 μg IMAB362 (zolbetuximab reference protein) 동등 Cmax. BNT142 1.4 mg/kg IV ≈ 2.5 mg/kg reference protein. xenograft 종양 모델에서 BNT142 0.1 μg ≈ 100 μg reference protein 동등 antitumor — mRNA-LNP가 일부 시나리오에서 더 적은 dose로 동등 효능 도달 가능성.

## 4. Implication for our LNP work

사내 mRNA-LNP encoded 단백질 / 항체 프로젝트의 FIH dose 결정에 직접 참조 가능한 framework. 핵심 가져갈 점: NHP single-species scaling으로 인간 PK 1.33-fold 이내 예측이 검증됐다는 점은 dose-finding 단계에서 NHP cohort 1개로 충분함을 시사 — 임상 진입 timeline 단축 + cost 절감.

구체적 design 기준 적용: allometric exponents (CL ~0.80, V1/V2 ~1, Q ~0.65, k_translate ~−0.51 from mouse / 0 from NHP, k_elim,mRNA ~−0.10) — 사내 internal PK report에 reference로 인용 가능. 마우스 4-fold 오차는 species translation efficiency 격차 큼을 시사하므로 early discovery는 마우스로 충분하나 dose-determination은 NHP 필수임을 운영 원칙으로 채택할 만함.

다만 본 framework은 **liver-mediated secretion 모델에 한정** — sinusoidal 발현 단백질이 systemic circulation으로 secreted되는 경로. spleen-tropic LNP, muscle-tropic LNP, intratumoral 발현 등 non-hepatic platform에서는 별도 framework 필요. 또한 항체 외 다른 secreted protein (e.g., 효소 보충요법) 으로 확장 시 V1/V2 default value 재설정 필요.

## 5. Limitations / open questions

- 학습 데이터셋 모두 liver-targeting iLNP (ApoE-LDLR 경로 hepatocyte 발현). spleen-tropic / muscle-tropic LNP에서 동일 exponents 작동 미검증.
- 외부 검증은 NHP-based scaling 1건 (mRNA-1944, 마우스 데이터 부재) — 마우스 single-species scaling의 외부 validation 없음.
- Antibody clearance assumes linear; target-mediated nonlinear elimination이나 saturable processes는 average behavior에 묻힘 — bispecific T-cell engager (RiboMab02.1)에서 잠재적 영향 미평가.
- Single dose PK only — repeated dosing immunogenicity (ADA), translation efficiency 감소, mRNA backbone-specific innate response 등 미모델링.
- Model parameter 추정 RSE 일부 high (e.g., k_elim,mRNA RSE 42% in BNT141, ktranslate RSE 12% in RiboMab02.1) — replication 부족, parameter 식별성 한계.
- 임상 cohort N 명시 없음 (descriptive statistics만 — geometric mean, %CV 등). 작은 cohort (Phase I/II dose-escalation) 영향 quantification 불가.
- 분석 시점 BNT141/142 모두 Phase I/II 진행 중 — Phase 2/3 expanded dataset에서 model 재검증 필요. 본 paper의 scaling 일반성 주장은 향후 추가 분자 (e.g., mRNA-3927 propionic acidemia, mRNA-6231 IL-2 mutein 같은 non-Ab payload)로 확장 검증 가치.

---

<details>
<summary>Abstract (raw)</summary>

Messenger RNA (mRNA)-lipid nanoparticle (mRNA-LNP) platforms enable the in vivo expression of almost any therapeutic protein, offering unprecedented flexibility for clinical translation. However, for these rapidly deployable therapies, predicting the first-in-human (FIH) dose remains a key challenge. We developed an allometric scaling framework for human pharmacokinetic (PK) prediction of antibodies expressed from intravenously administered mRNA-LNPs, leveraging preclinical and clinical data for BNT141 (encoding RiboMab01, a full IgG1) and BNT142 (encoding RiboMab02.1, a bispecific Fab-scFv-based T-cell engager). The dose-normalized Cmax (DCmax) and dose-normalized AUC (DAUC) of translated antibodies across multiple species could be described by the allometric approach, with the estimated exponents ranging from −1.29 to −1.42 for BNT141 and BNT142. We also determined generalized single-species allometric scaling exponents of −1.26 from mice and −0.75 from nonhuman primate (NHP), respectively, that enabled the human predictions of translated antibodies exposure approximately 4-fold (mice) and within 2-fold (NHP). A mechanistic cross-species translational model was further developed that integrated mRNA-specific elimination and translation efficiency parameters to characterize the exposure of the translated antibodies from mRNA-based therapeutics. The translational model could predict the human PK exposure of translated antibodies within 1.33-fold for BNT141 and BNT142 via single-species scaling from NHP parameters as well as capturing the concentration-time profiles with reasonably high fidelity. Validation with publicly available mRNA-1944 (encoding CHKV-24, full IgG1) data confirmed both the allometric scaling and translational modeling methods' robustness when scaling from NHP data. Taken together, these results support a generalized cross-species PK relationship that is independent of the molecular characteristics of the translated antibodies or antibody-like protein products. This integrated scaling and modeling framework offers a generalizable solution for accelerating FIH dose selection of mRNA-encoded therapeutic antibodies and is adaptable to other recombinant proteins of interest.

</details>
