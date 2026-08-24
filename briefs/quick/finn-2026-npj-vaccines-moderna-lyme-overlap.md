---
slug: finn-2026-npj-vaccines-moderna-lyme-overlap
title: "Monovalent and multivalent OspA mRNA-LNP vaccines elicit functional antibodies and protect against Borrelia burgdorferi in mice"
first_author: "Meredith B. Finn"
last_author: "Christina Dold"
journal: "npj Vaccines"
journal_abbr: null
year: 2026
doi: 10.1038/s41541-026-01451-7
url: https://www.nature.com/articles/s41541-026-01451-7
zotero_key: 2YYT8PSS
category: "LNP"
keep_tag: keep/LNP
generated_at: 2026-05-06
---

# Monovalent and multivalent OspA mRNA-LNP vaccines elicit functional antibodies and protect against Borrelia burgdorferi in mice

> Meredith B. Finn et al. (2026, npj Vaccines)  
> DOI: [10.1038/s41541-026-01451-7](https://doi.org/10.1038/s41541-026-01451-7) · Zotero: [`2YYT8PSS`](zotero://select/items/2YYT8PSS)

## 1. TL;DR

Moderna가 OspA mRNA-LNP Lyme 백신 — monovalent `mRNA-1982` + heptavalent `mRNA-1975` — 을 Phase 1/2 (NCT05975099)로 진입. 1.85 Å crystallography로 mRNA-encoded OspA ST1이 native fold + LA-2 epitope 유지를 확인 (PDB `9CDS`), C3H 마우스 tick-challenge에서 2-dose 0.2 µg 단독으로도 4/5 sterilizing protection, heptavalent 0.7 µg에서 5/5. 박테리아 surface lipoprotein이 mRNA-LNP platform에서 작동한다는 structural-to-clinical 패키지 — Moderna LNP 파이프라인이 viral·oncology를 넘어 transmission-blocking 인디케이션으로 다각화하는 신호.

## 2. Background & motivation

Lyme disease는 미국에서만 연간 47만 케이스로 추정 (CDC)되는 진드기-매개 spirochete 감염증으로, 미국에서는 *B. burgdorferi* sensu stricto, 유럽에서는 *B. garinii* / *afzelii* / *bavariensis* 등 다중 genospecies가 분포한다. OspA (Outer surface protein A, ~30 kDa lipoprotein)는 진드기 midgut에서 발현되는 spirochete 표면 단백질로 transmission-blocking 타깃으로 오랜 검증을 받아왔다. 1998년 GSK의 recombinant OspA subunit 백신 LYMErix가 출시됐으나 reactive arthritis 자가면역 mimicry 우려 + 시장 채택 부진으로 2002년 자진 철수, 이후 20여 년간 라이선스된 Lyme 백신은 부재 상태였다.

이 논문은 OspA를 mRNA-LNP로 인코딩하여 (a) multi-serotype 커버 + (b) subunit 백신 대비 native fold 보장 + (c) Phase 1/2 진입까지의 preclinical-to-clinical 패키지를 제시한다. 단순한 antigen 교체가 아니라 *bacterial surface lipoprotein이 mRNA-LNP platform에 적합한가*를 immunology + structural biology 양쪽에서 첫 검증한 사례라는 점에서 mRNA platform indication expansion의 reference 사례로 의미가 있다. LNP 조성은 ionizable lipid:DSPC:cholesterol:PEG-lipid = **50:10:38.5:1.5 mol%**, 입자 80–100 nm, >90% encapsulation, <10 EU/mL endotoxin (ionizable lipid 명칭은 Moderna 비공개).

## 3. Key findings

- **Crystallography (ST1 only)**: mammalian-expressed OspA ST1을 neutralizing mAb LA-2 Fab와 복합체로 1.85 Å 해상도 결정 (PDB `9CDS`); Cα RMSD <2 Å vs bacterially-expressed reference 구조 (PDBs 7JWG / 2G8C / 1OSP / 1FJ1). Octet BLI로 LA-2 (Kd 27.7 ± 1.0 nM), 184.1 (84.9 ± 8.1 nM), 857-2 (4.4 ± 0.1 nM) 3종 neutralizing mAb 결합 확인 — *"three neutralizing mAbs … each directed against distinct regions of OspA"*. 추가로 hLFA-1 T cell epitope (165–173, YVLEGTLTA → FILEGRFTA: Y165F/V166I/T170R/L171F) 변이 도입.
- **In vitro functional**: C3H 마우스 day 1+21+42 IM 면역 (Fig 1, n=9-10/group → Nterm-TM lead 선정), heptavalent functional comparison Fig 3 n=10/group. SBA reporter strain *B. burgdorferi* B31-5A4 (GGW979, mScarlet-I) + 20% guinea pig complement, 50% MFI reduction 기준. **mRNA-LNP arm SBA titer 1:800–1:51,200 vs Recombitek+alum 1:100–1:3,200**. 결정적으로 *"sera from mice vaccinated with the ST1-7 protein cocktail had no detectable bactericidal activity, even though the serum-derived antibodies were capable of recognizing OspA"* — recombinant protein은 binding은 되지만 borreliacidal activity 부재 → mRNA-LNP가 functional antibody 유도에서 우위.
- **Multivalent non-interference**: n=7/group, day 1+21 IM, day 36 serum. 1 µg monovalent ST1 vs **3.5 µg heptavalent (0.5 µg/ST)** vs 7 µg recombinant ST1-7 protein (1 µg/ST). 결과: *"the levels of OspA ST1 antibodies elicited by the heptavalent OspA ST1-7 mRNA-LNP vaccine were not significantly different than the monovalent OspA ST1 mRNA-LNP vaccine"* + LA-2 equivalent antibody 동등. 단 IgG subclass breakdown은 보고 안 됨 (Luminex total IgG only). Heptavalent vs recombinant protein은 p<0.0001로 mRNA-LNP 우세.
- **Tick-mediated challenge** (Table 2): C3H/HeN 마우스, 5 *Ixodes scapularis* nymph 챌린지 (B. burgdorferi B31, ~75-90% infection rate), final dose 후 2주 post-challenge, **n=5/group**. 2-dose **0.2 µg ST1 → 4/5 protected** (1 culture+, 0 serology+); 3-dose 0.2/0.5/1.0 µg → **5/5 protected**; 2-dose heptavalent 0.7 µg (0.1 µg/ST) → 5/5 culture-negative; dose 내림 → 0.05 µg → 4/5; **0.01 µg → 1/5 (4/5 infected)** — minimum protective dose 약 0.05 µg. Control (PBS, NTFIX) → 5/5 infected.
- **Phase 1/2 NCT05975099**: monovalent `mRNA-1982` + heptavalent `mRNA-1975` 동시 진행. 논문에는 *"Persistence of immunogenicity and functional antibody responses is being assessed in the ongoing Phase 1/2 clinical study"* 문구만, dose level / endpoint / readout date 미공개.

## 4. Implication for our LNP work

Moderna가 mRNA-LNP를 viral·oncology 외 *bacterial surface antigen + transmission-blocking* 인디케이션으로 확장한 첫 임상 사례. 우리 LNP 파이프라인 관점에서 세 가지 가져갈 점:

1. **Multi-domain bacterial protein이 mRNA-LNP에서 native fold 회복 가능** — 30 kDa OspA가 작동했다는 structural validation은 우리가 mRNA-encoded antigen 후보를 검토할 때 약한 양성 신호 (단, lipoprotein 특이 acylation은 mammalian cell에서 재현되지 않을 수 있음 — fulltext에서 PTM 검증 여부 확인 필요).
2. **Multi-cistron multi-serotype LNP가 immune interference 없이 단일 dose로 가능**하다는 점은 multi-antigen LNP 설계 시 cargo ratio 최적화의 reference (예: 7가지 mRNA를 어느 mass ratio로 packaging했는지가 핵심 노하우).
3. **Non-viral, non-oncology mRNA 백신 임상 진입 = LNP platform 인디케이션 시장 확장의 trigger** — transmission-blocking 컨셉은 말라리아·뎅기·chikungunya 등 vector-borne 영역으로 확장 가능. 이 방향성은 mRNA-LNP supplier·CMO·CRO 생태계에 시장 기대치를 올린다.

경쟁 포지셔닝 측면에서 Lyme은 단독 commercial market은 작지만 (LYMErix 철수 사례) Moderna로서는 R&D portfolio 다양성 + regulatory pathway 확보의 strategic move로 해석하는 것이 합리적. 우리 입장에서는 mRNA-LNP에 진입하는 transmission-blocking 백신 컨셉이 academic novelty 단계를 벗어나 임상 가능성을 보여줬다는 점을 트래킹. **추가 시사점**: minimum protective dose가 sub-microgram (0.05–0.2 µg) 영역까지 내려간 점은 multi-cistron mRNA-LNP에서 dose-sparing 가능성의 강한 양성 데이터 — 우리 multi-antigen LNP 설계 시 dose budget 추정에 직접 활용 가능.

## 5. Limitations / open questions

- **LYMErix HLA-DR4 reactive arthritis mitigation**: 저자들은 platform-based 논거가 아닌 **engineering-based** 회피 — hLFA-1 T cell epitope (165–173)을 Y165F/V166I/T170R/L171F로 치환. *"despite prior reports linking this epitope to antibiotic-refractory Lyme arthritis having been conclusively disproven"*이라며 precautionary substitution임을 명시. mRNA-LNP가 subunit과 어떻게 다른지 mechanism-level 비교는 부재 → Phase 1/2 safety readout이 가장 중요한 watchpoint.
- **Long-term durability 미평가**: *"Durability of protection was not evaluated in the present study, as animals were challenged at peak immunogenicity"* — 챌린지가 final dose 후 2주 시점에서만 진행됨. 6개월+ titer decay, booster 효과는 모두 NCT05975099 임상에 deferred. multi-cistron mRNA-LNP의 long-term durability는 미지수.
- **ST2-7 structural fold 미검증**: crystallography는 ST1만 (PDB `9CDS`). ST2-7는 conserved-epitope mAb 857-2 binding으로만 fold inference. 다른 ST의 LA-2 epitope 보존 여부는 indirect 확인.
- **Co-infection scenario 부재**: Anaplasma phagocytophilum, Babesia microti, Powassan virus 등 진드기 매개 co-infection에 대한 언급 없음. 인간 자연감염은 종종 co-infection이며, OspA-only 백신의 real-world 효능은 이 시나리오에서 제한될 수 있음.
- **Lipidation 의도적 제거 — TLR2 self-adjuvant 상실**: *"we engineered an mRNA sequence lacking the first 25 N-terminal residues, which encompass the lipidation motif not processed in mammalian systems"*. 즉 mRNA-encoded OspA는 truncated (lipidation 부재). 저자 주장: *"the mRNA-LNP delivery can compensate for the lack of lipidation"*. 그러나 LNP-as-adjuvant가 native lipidated OspA의 TLR2 agonism과 quantitatively equivalent한지는 head-to-head head-to-head로 입증되지 않음 — mRNA-LNP 우위가 결국 LNP 자체의 innate response인지, 발현된 antigen의 fold quality 차이인지 deconvolution 안 됨.

---

<details>
<summary>Abstract (raw)</summary>

Outer surface protein A (OspA) is a ~30 kDa lipoprotein displayed on the surface of Borrelia burgdorferi sensu lato, the etiological agent of Lyme disease. Here we report on the preclinical evaluation of OspA-encoding nucleoside-modified mRNA lipid nanoparticle (OspA mRNA-LNP) vaccines for the prevention of Lyme disease. Crystallographic and binding studies using a panel of transmission-blocking antibodies confirmed that the mRNA-encoded OspA serotype 1 (ST1) expressed in mammalian cells assumes its native structure and retains known protective epitopes. Immunization of mice with OspA ST1 mRNA-LNP elicited functional serum antibodies that promoted spirochete agglutination and complement-dependent borreliacidal activity in vitro. We also examined the impact of combining ST1 OspA mRNA with OspA STs 2-7, which are associated with predominant Borrelia genospecies in Europe (B. garinii, B. afzelii, and B. bavariensis). The additional six STs mRNA did not interfere with ST1 antibody titers and functionality. Finally, mice vaccinated two or three times with different dose levels of OspA ST1 mRNA-LNP or with the heptavalent mRNA vaccine were protected against B. burgdorferi infection in a tick-mediated challenge model. The monovalent and the heptavalent OspA mRNA vaccines (mRNA-1982 and mRNA-1975, respectively) are currently undergoing testing in a Phase 1 clinical trial (NCT05975099).

</details>
