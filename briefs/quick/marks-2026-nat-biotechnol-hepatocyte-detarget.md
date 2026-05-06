---
slug: marks-2026-nat-biotechnol-hepatocyte-detarget
title: "mRNA vaccine immunity is enhanced by hepatocyte detargeting and not dependent on dendritic cell expression"
first_author: "Adam Marks"
last_author: "Brian D. Brown"
journal: "Nature Biotechnology"
journal_abbr: "Nat Biotechnol"
year: 2026
doi: 10.1038/s41587-026-03099-z
url: https://www.nature.com/articles/s41587-026-03099-z
zotero_key: VSFPIPVQ
category: "LNP"
keep_tag: keep/LNP
generated_at: 2026-05-06
---

# mRNA vaccine immunity is enhanced by hepatocyte detargeting and not dependent on dendritic cell expression

> Adam Marks et al. (2026, Nature Biotechnology)  
> DOI: [10.1038/s41587-026-03099-z](https://doi.org/10.1038/s41587-026-03099-z) · Zotero: [`VSFPIPVQ`](zotero://select/items/VSFPIPVQ)

## 1. TL;DR

mRNA-LNP 백신의 면역원성은 **pAPC 직접 발현이 dispensable**하고 (i.m. SARS-CoV-2 Spike CD8 priming WT vs 142T 차이 없음), 대신 **muscle injection site myocyte → cross-presentation**이 antigen depot로 작동. 반대로 i.v. 후 hepatocyte 발현은 PD1/PDL1 매개로 antigen-specific T cell을 억제 — mRNA UTR에 **miR-122 target (122T) 4× 삽입**으로 hepatocyte 발현 95% 차단 시, GFP-specific CD8+ T cell 10% → 28% (3-fold↑), A20-GFP lymphoma 종양 부피 추가 50%↓. Anti-PD1로 차이 abolish → 기전 직접 실증.

## 2. Background & motivation

mRNA-LNP는 i.v.에선 hepatocyte 우세, i.m.에선 myocyte + dLN pAPC + 일부 hepatic leak으로 **다양한 cell type을 transfect**한다. 그러나 어느 cell이 mRNA를 직접 번역해야 효과적 T-cell priming이 일어나는지는 미정의 — 기존 DC depletion 실험은 antigen presentation까지 함께 막아 confound이 있었다 (DC가 직접 발현해서 priming하는지, 다른 cell의 항원을 받아서 priming하는지 분리 불가).

본 연구는 **synthetic miRNA target site (miRT)** 도구로 confound을 제거: mRNA UTR에 cell-type-specific miRNA target sequence를 삽입하면 해당 cell에서만 mRNA가 RISC-mediated degradation → DC 자체나 LNP 화학은 건드리지 않고 cell-intrinsic mRNA 발현만 끔. 사용된 miRT: 122T (hepatocyte, miR-122), 142T (hematopoietic/pAPC, miR-142-3p), 133T+206T (skeletal myocyte, miR-133·miR-206), 155T (activated mac/DC, miR-155). LNP는 SM-102 ionizable lipid 표준 처방.

## 3. Key findings

- **122T copy-number-dependent silencing, modification-independent**: AML12 hepatocyte에서 1× 122T → GFP 50%↓, 4× 122T → >95% silencing. ΨU, m5C, N1m 변형 mRNA에서도 동등한 silencing (i.e., modified base와 RISC mediated degradation은 충돌 없음). In vivo i.v. 20 μg 단일 도즈에서 **150-fold 감소** (~800 GFP+ hepatocyte/mm² WT vs <20 with 122T), 3× 반복 i.v.에도 escape 없음. Liver macrophage·endothelial cell은 GFP+ 유지 → **cell-type-specific**

- **pAPC silencing (142T) → IM 백신 면역원성 무영향**: SARS-CoV-2 Spike i.m. (C57BL/6, 5 μg × 2회, n=4/grp) — Spike-specific CD8+ T cell WT vs 142T 차이 없음. OVA·GFP system에서도 동일 또는 경미한 감소만 (GFP CD8 10% → 5%). 96-plex Olink + RT-qPCR로 cytokine/chemokine 패널 (CXCL9, CCL2/3/5, IL-10, TNF, CSF2) 확인 — innate adjuvant 활성도 WT와 동등. **DC 직접 mRNA 발현은 dispensable**

- **Cross-presentation/cross-dressing 직접 실증**: WT CD45.1+ BM → Ai14 chimera에서 Cre RNA-LNP i.v. 후 liver pAPC의 10–20%가 tdTomato+ (자체 tdTomato gene 없음 → hepatocyte로부터 antigen uptake). 122T 처리 시 liver tdTomato+ pAPC 소실. Spleen에서는 122T로도 1–2% pAPC가 tdTomato+ → non-hepatocyte non-hematopoietic source 존재. C2C12 myocyte + RAW macrophage 공배양: myocyte를 142T로 transfect해도 ~12% macrophage GFP+ → **muscle cell이 단백질 antigen을 release하여 pAPC가 uptake**

- **Hepatocyte detargeting (122T) → CD8 response 3x↑, A20 lymphoma 부피 추가 50%↓**: BALB/c i.v. 3-dose (20 μg, day 0/5/20) → GFP-specific CD8 10% (WT) vs 28% (122T). 항체 titer는 비차이. A20-GFP lymphoma s.c. 모델 + i.v. 4-dose (day 4/7/11/15, n=5/cohort, 2× 독립 반복) — WT 대비 122T가 종양 volume 추가 50% 감소. TIL의 GFP-specific CD8가 **less exhausted** (TIM3+PD1+ 빈도 ↓, TIM3·PD1 MFI ↓), CD44+/IFNγ+/granzyme B+ effector 마커 ↑

- **Mechanism = PD1/PDL1**: Anti-PD1 동시 투여 시 RNA.WT vs 122T의 antigen-specific CD8 차이 **abolish** (Fig 4l, n=5). Granzyme B+ CD8도 동일 — IgG isotype에서는 122T 우월, anti-PD1에서는 평준화. Hepatocyte 발현 자체가 PD1/PDL1 axis를 통해 antigen-specific T cell dysfunction 유도

- **Myocyte는 IM 백신의 antigen depot**: 133T+206T 결합 i.m. → skeletal myocyte silencing 시 GFP-specific CD8 + Spike-specific CD8 + granzyme B 모두 감소 (n=4/grp). 항체 titer는 유지 → **세포면역과 항체면역의 cell-type-specific 분리 가능**. IM 백신에서 myocyte 발현이 CD8 priming의 주요 antigen 공급원임을 직접 입증

- **122T는 pre-existing T cell 매개 hepatotoxicity 차단**: GFP-reactive Jedi CD8 T cell 입양이전 + GFP RNA-LNP — WT는 liver CD8 infiltration ↑, serum ALT/AST ↑, cleaved caspase-3+ apoptotic hepatocyte ↑. 122T는 모두 baseline 회복. hCD19-CAR-T + hCD19 RNA system도 동일 — **CAR-T target을 mRNA로 boosting할 때 hepatocyte off-target killing 차단**

## 4. Implication for our LNP work

가장 큰 함의는 **LNP composition (SM-102, PEG-lipid, ionizable, helper)을 그대로 두고 mRNA cargo UTR에 4× 122T만 추가**하는 mRNA-side fix로 hepatocyte 발현 95% 차단 + 면역원성 유지 + hepatotoxicity 위험 동시 차단이 가능하다는 점이다. Platform-level 변경 비용이 없어 사내 mRNA-LNP 백신·치료제 cargo 표준에 거의 free로 얹을 수 있다. 특히 i.v. 종양 백신 (A20 lymphoma 결과 그대로 적용 가능) 및 mRNA로 CAR-T·TCR-T를 boosting하는 적응증, Cas9·base editor mRNA 등 pre-existing T cell immunity 위험이 있는 cargo에서 가치가 크다.

부수적으로, **IM 백신에서 pAPC 직접 표적성을 추구하는 LNP 화학 (spleen-tropic ionizable lipid, mannose-decoration, LN-draining size tuning)의 우선순위를 재검토**할 근거가 된다 — myocyte cross-presentation 경로가 충분히 강력해 pAPC 직접 발현 손실을 보상함이 i.m. SARS-CoV-2 Spike 모델에서 직접 입증됨. 단, 본 연구의 cross-presentation 증거는 mouse + in vitro/in vivo 한정이므로 인간 muscle 맥락 (특히 노령·면역저하 population) 재검증은 별도 작업이다. 또한 **myocyte silencing이 CD8는 감소시키지만 항체는 유지** — 항체 vs 세포면역 반응을 cell-type miRT 조합으로 tuning할 수 있다는 platform-level design degree of freedom을 시사.

## 5. Limitations / open questions

- **Species translation gap**: miRNA seed conservation은 mouse-human 일치하나 절대 abundance가 다름 — 특히 hepatocyte miR-122는 인간에서 충분히 풍부할 것으로 예상되지만, miR-142-3p (pAPC) 효율은 인간 dataset 별도 검증 필요. miR-133·miR-206 (skeletal muscle)도 species-specific abundance 검토 항목
- **단일 tumor 모델 한정**: A20-GFP B-cell lymphoma는 면역원성 강한 hematologic tumor. Cold/poorly immunogenic solid tumor (pancreatic, glioma 등)에서 hepatocyte detargeting 효과의 일반화 여부 미검증
- **PD1/PDL1 "largely"**: anti-PD1로 difference abolish되긴 하나 잔여 기전 미정 — Liver-resident Treg, Kupffer cell IL-10, LSEC 면역관용 환경 등이 어떻게 기여하는지 후속 mechanistic. Anti-PD1 비반응자에서의 hepatocyte detargeting 효과도 미평가
- **mRNA stability/번역 효율 trade-off 미정량**: 4× 122T UTR 삽입의 protein yield cost (mRNA half-life, ribosome occupancy, modified base × miRT 상호작용)와 immunogenicity의 net balance를 paper에서 정면으로 다루지 않음. Cargo 별도 optimization 필요
- **CMC/regulatory burden**: UTR-modified mRNA는 IND-enabling characterization (sequence verification, modified-base ratio, in vitro miRT functional assay, off-target seed match 검토)가 추가됨. 임상 진입 비용 미논의
- **Cross-dressing 분자 메커니즘 미해상**: myocyte → pAPC antigen transfer가 secreted protein endocytosis인지, exosome-mediated shedding인지, MHC-I peptide direct transfer (cross-dressing)인지 분리 부족. 후자라면 antigen processing pathway 우회로 가능 → vaccine design에 다른 의미
- **장기 안전성 데이터 부재**: 3× 반복 i.v.까지만 검증, 만성 투여 (e.g., RNA replacement therapy) 시 122T 효율 유지 여부 + miR-122 sponge 효과 (의도치 않은 endogenous miR-122 sequestration → liver 대사 영향) 평가 없음

---

<details>
<summary>Abstract (raw)</summary>

Proteins encoded by mRNA vaccines can be expressed by a diversity of transfected cell types but how cell-type-specific expression influences immunity is poorly understood. To investigate this, we incorporated synthetic microRNA target sites (miRT) into lipid nanoparticle (LNP)-delivered mRNA vaccines to silence mRNA expression specifically in professional antigen-presenting cells (pAPCs), hepatocytes or myocytes. We found that mRNA expression in pAPCs was dispensable for priming antigen-specific T cells, whereas mRNA expression in myocytes induced similar or stronger immune responses, including for SARS-CoV-2, suggesting that antigen cross-presentation or cross-dressing may be more impactful than direct mRNA expression in pAPCs. In contrast, mRNA expression in hepatocytes suppressed the antigen-specific T cell response, partly through PD1/PDL1. In mice bearing tumor-associated antigen (TAA)-expressing lymphoma cells, miRT-mediated hepatocyte-silenced TAA mRNA vaccine enhanced immune response and reduced tumor burden. Thus, non-pAPC expression shapes immunity to mRNA-encoded protein and inclusion of miRTs can boost or blunt mRNA-LNP immunogenicity.

</details>
