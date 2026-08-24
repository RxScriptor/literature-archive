---
slug: dirisala-2026-nojournal-liver-stealth-presoak
title: "2-arm-PEG-oligocations transiently shield the liver sinusoids to mitigate off-target hepatic expression of mRNA lipid nanoparticles"
first_author: "Anjaneyulu Dirisala"
last_author: "Satoshi Uchida"
journal: "bioRxiv (preprint)"
journal_abbr: null
year: 2026
doi: 10.64898/2026.04.29.721537
url: https://www.biorxiv.org/content/10.64898/2026.04.29.721537v1
zotero_key: C6626N4I
category: "LNP"
keep_tag: keep/LNP
generated_at: 2026-05-07
suitability: internal-only
preprint: true
---

> ⚠️ **internal-only**: Moderna / Acuitas / Arcturus 모두 풀고 있는 hepatic detarget 영역에 직접 informative. **Public `literature-archive` repo에 commit 금지**. 검토 후 dds-work 또는 briefing-dashboard 같은 Private 위치로 이동 권장.
> 📄 **preprint** (2026-05-01 posted, peer review 미통과). 데이터 검증 후 재평가 필요.

# 2-arm-PEG-oligocations transiently shield the liver sinusoids to mitigate off-target hepatic expression of mRNA lipid nanoparticles

> Anjaneyulu Dirisala et al. (2026, bioRxiv preprint, Kataoka & Uchida labs)  
> DOI: [10.64898/2026.04.29.721537](https://doi.org/10.64898/2026.04.29.721537) · Zotero: [`C6626N4I`](zotero://select/items/C6626N4I)

## 1. TL;DR

iLNP **자체 변형 없이** 사전 IV 주입 (5분 전)으로 liver sinusoidal endothelial (LSE) wall을 2-arm-PEG-oligocation으로 일시적 stealth-coat → ALC-0315 iLNP의 hepatic protein 발현 22-fold 감소 + spleen 2.3-fold 증가 (50-fold spleen selectivity). MC3 LNP에도 41-fold liver 감소로 generality 확인. 백신 (OVA mRNA) ELISpot IFN-γ 2.5-fold 향상 + IL-12 i.t. cytokine 치료에서 hepatic IL-12 leak 감소하면서 antitumor 유지. 2-arm-PEG-OligoOrn은 이미 siRNA/ASO Phase I 임상 carrier로 진입 — 임상 친화 plug-and-play strategy.

## 2. Background & motivation

iLNP의 본질적 liver tropism은 mRNA 백신·면역치료의 안전성·효능 양쪽을 압박. Hepatic 누적 메커니즘은 **다중**: (1) ApoE-bound iLNP가 LDLR로 hepatocyte uptake, (2) Kupffer cell + LSEC 의 강한 scavenging, (3) sinusoidal slow flow. 단일 receptor 차단으로 풀리지 않음. 기존 우회 전략 한계: scavenger receptor ligands는 toxicity 우려, dextran sulfate / decoy liposome은 prior work에서 hepatic clearance 차단 실패.

Pre-existing autoimmune hepatitis 사례 (COVID-19 mRNA 백신 후 spike-targeting CTL의 간 침윤) + i.t. cytokine 치료에서 leak-driven systemic toxicity 둘 다 hepatic off-target expression 줄이는 generic approach 필요성 시사. 본 연구는 LSE wall 자체를 PEG로 비특이적 broad mechanism 차단하는 strategy 제시 — 이미 임상 검증된 carrier (2-arm-PEG-oligocation, siRNA/ASO Phase I 사용 중) 활용.

## 3. Key findings

- **iLNP characterization**: ALC-0315 iLNP 직경 83.8 ± 0.7 nm, PDI 0.09 ± 0.02, ZP −5.8 ± 1.7 mV, EE 95.7 ± 0.8%. 2-arm-PEG carrier: 40 kDa PEG × 2 arms + OligoLys (~20 lysine units) 또는 OligoOrn. FCS 측정 결과 bloodstream 내 iLNP와 직접 상호작용 없음 (diffusion time 270 vs 286 μsec, n=11/18).
- **Biodistribution (ALC-0315, 5min pre-injection, 4h endpoint)**: hepatic luciferase 22-fold 감소, splenic 2.3-fold 증가, **spleen-to-liver ratio 0.13→6.1 (50-fold spleen selectivity)** (n=5). 24h endpoint: 0.78→21 (28-fold). lung/kidney/heart/brain 영향 없음. AST/ALT/BUN/creatinine/LDH 24h 정상.
- **Cellular-level shift (Cre/Ai9 reporter, 3d endpoint, n=3)**: iLNP only — hepatocyte tdTomato ~100%, KC + LSEC 각 ~20%. Pre-injection — hepatocyte 유의 감소, KC + LSEC near-background. 동시 splenic CD11c+ DC tdTomato 증가. **iLNP 자체는 그대로 두고 cellular target만 hepatocyte→splenic DC로 shift.**
- **Generality (다른 ionizable lipid + 다른 oligocation)**: MC3 iLNP (105.4 ± 6.5 nm, EE 82.0 ± 3.1%) — 41-fold hepatic 감소 + 2.8-fold splenic 증가, >100-fold spleen selectivity. OligoLys → OligoOrn 치환 — 28-fold hepatic 감소, 2.6-fold splenic, >100-fold selectivity. **2 ionizable lipid × 2 oligocation = 4 조합 모두 작동.**
- **Vaccination 응용 (ALC-0315/OVA mRNA, IV systemic, 2-week interval prime-boost, n=4-5)**: ELISpot IFN-γ spot 약 2.5-fold 증가 (booster 1주 후); in vivo CTL assay 1 μg mRNA dose에서 CTL activity 유의 향상. **Spleen redirect + hepatic immune tolerance 회피 두 메커니즘 동시 기여 가설**.
- **Cytokine therapy 응용 (IL-12 mRNA i.t. 종양 내)**: 사전 OligoOrn IV로 hepatic IL-12 발현 + systemic IL-12 노출 감소하면서 antitumor 유지. i.t. injection이 systemic circulation으로 leak되는 일반적 우려 완화 — IL-12 systemic toxicity는 임상 진입 큰 장애였던 점 고려 시 응용 가치 높음.
- **임상 friendliness**: 2-arm-PEG-OligoOrn은 이미 siRNA/ASO Phase I 임상 carrier (NCT 다수 cited). 본 paper의 strategy는 현재 임상 LNP product에 carrier protocol 추가만으로 적용 — LNP 재formulation 없음.

## 4. Implication for our LNP work

가장 매력적인 점은 **LNP backbone 변경 없이** pre-injection만으로 hepatic detarget 달성. 사내 LNP 라인업 (어떤 ionizable lipid이든) 그대로 두고 spleen/lymph node-tropic 백신 또는 i.t. cytokine 안전성 개선이 가능 — plug-and-play 컨셉. ALC-0315 + MC3 두 backbone 동일 작동 검증된 점이 generalizability 핵심 신호.

가져갈 design 기준: (1) sequential dosing protocol (5min pre-injection)은 임상 운영 부담 작음 — IV cocktail 형태로 simple. (2) 2-arm-PEG-oligocation carrier가 이미 siRNA/ASO 임상 carrier 진입 — 새 carrier 개발 부담 없이 license-able material. (3) spleen redirection이 자동 따라옴 — 단순 hepatic detarget 이상의 splenic immunization 강화 효과. (4) i.t. cytokine 프로젝트 (IL-12, IFN, TNF 등) 가 있다면 leak-driven systemic toxicity 직접 mitigation tool로 즉시 평가 가능.

비교 가치: SORT (Siegwart 그룹), GalNAc decoy (Acuitas/Alnylam), ionizable lipid 재디자인 등 기존 hepatic detarget 전략과 본 strategy를 같은 백신·치료 모델에서 head-to-head로 비교한 데이터는 없음. 사내에서 2-3개 strategy 동시 평가 시 본 paper의 carrier를 control arm으로 포함 가치.

**가장 큰 caveat**는 preprint라는 점 — Nat Biotechnol/Biomed Eng급 peer review를 통과해야 figure 신뢰도 확정. Kataoka 그룹의 prior work (2-arm-PEG-OligoLys LSE coating 공저 paper 62, 63) 가 peer-reviewed라는 점은 위안 신호.

## 5. Limitations / open questions

- 마우스 only — 인간 LSE wall 구조 (sinusoid 직경, fenestration 80-150 nm) + heparan sulfate proteoglycan 분포는 마우스와 다를 수 있음. NHP 데이터 없음.
- Spleen redirection은 splenic open circulation (red pulp F4/80+ macrophage 영역) bypass 메커니즘에 의존 — 인간 spleen에서도 동일 작동할지 미검증.
- 5min pre-injection timing은 결정 — 1min, 30min, 1h 등 다른 interval의 effect 데이터 부재. 임상 운영 (IV line 분리 vs 동시 cocktail) 결정 필요.
- 24h safety 단기 평가 only — 반복 투여 (vaccine prime-boost regimen 반복) 시 누적 효과, biliary excretion saturation, immunogenicity (anti-PEG ADA 등) 평가 없음.
- 2-arm-PEG (40 kDa × 2 arms = 80 kDa polymer payload) 자체는 large polymer — 다양한 liver function 환자 (cirrhosis, hepatic impairment) 에서 PK 변동 영향 미평가.
- LSE wall coating은 자연 면역 surveillance (Kupffer cell phagocytosis)을 일시 차단 → 동시 다른 감염 / 약물 hepatic clearance에 영향 가능성. Drug-drug interaction (특히 hepatically cleared drug) 미평가.
- IL-12 mRNA 외 다른 cytokine (IFN-α/γ, TNF, IL-2 등) 에서도 동일 leak-mitigation 작동할지 미검증.
- N: biodistribution n=4-6, vaccine ELISpot n=4, CTL assay n=5 — modest. 독립 코호트 replication 없음.
- preprint, peer review 미통과 (2026-05-01 posted). 동일 그룹의 prior peer-reviewed work (ref 62, 63 — 2-arm-PEG-OligoLys LSE coating viral vector + polymeric NP context) 는 안정적이나 본 paper의 iLNP-specific 결과는 추가 검증 필요.

---

<details>
<summary>Abstract (raw)</summary>

Ionizable lipid nanoparticles (iLNPs) are powerful platforms for mRNA based vaccines and immunotherapies; however, their intrinsic liver tropism compromises both safety and efficacy. Off-target hepatic protein expression from delivered mRNA raises safety concerns, and hepatic clearance limits efficient iLNP delivery to target organs. In this study, we address these challenges in mouse models by stealth-coating the liver sinusoidal endothelial (LSE) wall, the primary gateway for nanoparticle entry into the liver. Specifically, oligocations conjugated with two armed PEG (2 arm PEG oligocations), a clinically relevant material used in oligonucleotide delivery trials, were employed to transiently anchor PEG to the LSE wall with balanced affinity, ensuring robust coating followed by gradual biliary clearance. This approach reduced hepatic protein expression from iLNPs, subsequently administered either systemically or locally, by more than tenfold. Importantly, the strategy preserved iLNP accumulation in the spleen, a key target organ for vaccines, effectively redirecting iLNPs from the liver to the spleen. Consequently, in vaccine applications, pre-injection of the 2 arm PEG oligocation preserved or even enhanced vaccination efficacy while minimizing concerns associated with antigen expression in the liver. In applications involving cytokine mRNA therapy, specifically intratumoral interleukin 12 (IL 12) mRNA administration, systemic pre-injection of the 2 arm PEG oligocation successfully reduced off-target hepatic IL 12 expression and subsequent systemic IL 12 exposure, while maintaining antitumor efficacy. Collectively, these results demonstrate that LSE-wall stealth coating is a generalizable strategy to improve both the safety and efficacy of iLNP-based mRNA vaccines and immunotherapies.

</details>
