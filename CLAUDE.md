# literature-archive — Literature Brief Portfolio

> 위치: `literature-archive/CLAUDE.md`
> Layer: 2A (Brand, Public)
> 역할: 엄선된 논문 브리핑 포트폴리오 (Tier 2)
> 연결: rxscriptor-literature (Tier 1 수집·요약) → 이 repo (큐레이션)

---

## 1. Repo 목적

**논문 브리핑 포트폴리오 + 대시보드** (정적 사이트, Public)
- 박준영님이 **엄선한** 주요 논문의 1-page 브리핑
- 대시보드에서 검색·필터·분류
- 공개 포트폴리오 — 전문성·큐레이션 감각 보여주기
- 배포: GitHub Pages

**구분 주의**:
- `literature-archive` (이 repo): 큐레이션된 공개 포트폴리오
- `rxscriptor-literature` (별도): Streamlit DOI→요약 + Zotero crawling 도구
- 관계: rxscriptor-literature가 수집·필터, literature-archive가 결과물 공개

---

## 2. 2-tier brief 정책 (2026-05-06~)

- **Long-form HTML brief** — 매거진형 portfolio piece. 수동 작성, 인포그래픽 필요, dashboard 등록. Tier 2 큐레이션 결과.
- **Quick Markdown brief** — `briefs/quick/{slug}.md`. zotero-curate KEEP → `태그` 후속에서 auto-generated. 동료 이메일 배포용 lightweight 산출물. 인포그래픽·dashboard 등록 없음. 후일 long-form으로 승격 가능.

---

## 3. 브리핑 작성 표준 (절대 준수)

### 3-1. 슬러그 규칙 (v2, 2026-05-06~)

```
{firstauthor}-{year}-{journal-abbr}-{topic}
```

**예시**:
- Marks et al. 2026, Nat Biotechnol, mRNA hepatocyte detargeting → `marks-2026-nat-biotechnol-hepatocyte-detarget`
- Jo et al. 2026, Nature, mRNA CD8 → `jo-2026-nature-mrna-cd8`
- Lobb et al. 2026, JCR, i.v. LNP → `lobb-2026-j-control-release-iv-lnp`

**규칙**:
- 성 소문자
- year 4자리
- journal-abbr: Zotero `journalAbbreviation` 필드 → lowercase, dots/colons 제거, 공백 → 하이픈
- topic: 1-2 핵심 키워드, 하이픈 구분
- 전부 소문자

**v1 슬러그 (grandfathered)**: `{firstauthor}-{topic}-{year}` — 2026-05-06 이전 작성된 `jo-mrna-cd8-2026.html`, `lnpdb-2026.html` 그대로 유지. 신규 brief는 v2로.

### 3-2. 파일 배치

Long-form = `briefs/{slug}.html` + `assets/infographic/{slug}.png`, quick = `briefs/quick/{slug}.md`.

SVG 초안, preview 파일은 로컬 임시 폴더만 (repo에 커밋 금지).
Quick brief는 인포그래픽·dashboard 등록 없음 — 동료 이메일 배포용 lightweight 산출물.

### 3-3. Git 커밋 메시지

```
Add: {topic} brief ({primary-tag})
```

예: `Add: mRNA-CD8 priming brief (vaccine)`
Quick brief는: `Add: quick brief — {slug}` (예: `Add: quick brief — marks-2026-nat-biotechnol-hepatocyte-detarget`)

---

## 3a. Quick Markdown brief 표준 (auto-generated, 2026-05-06~)

이메일 배포·자동 chain용 lightweight brief. zotero-curate skill의 `태그 keep` 후속 단계에서 scaffold(frontmatter + 빈 5섹션)를 만들고 Claude가 5섹션을 채움. (전용 헬퍼 `lib/zotero_to_brief.py`는 **아직 미구현** — 현재는 zotero-curate skill이 직접 scaffold 작성. 본 repo에 `.py` 파일 없음.)

### 위치
`briefs/quick/{slug}.md` (slug v2, §3-1)

### 구조 (frontmatter + 5섹션, 고정)

형식은 기존 brief를 그대로 따른다 — canonical 예시 `briefs/quick/marks-2026-nat-biotechnol-hepatocyte-detarget.md`.
5섹션 = TL;DR / Background & motivation / Key findings / Implication for our LNP work / Limitations & open questions.

### 작성 원칙
- 한국어 primary, 과학·의학 용어 영문 병기 (전사 CLAUDE.md §2 따름)
- 본론 우선, 서두 garnish 금지
- §4 implication에서 회사 보안 게이트 (회사명·내부 코드명 절대 금지)
- **§3 Key findings + §5 Limitations는 fulltext 기반 작성이 디폴트**. abstract만으로 작성 시 §3에 specific data (N, %, miRNA seed, assay 명) 누락되고 §5는 design critique 대신 generic limitation에 그침. PDF attachment가 Zotero에 있으면 helper `--fulltext` 플래그로 indexed text를 sidecar fetch
- abstract만으로 작성한 bullet은 명시 표시 (`(abstract only — full text 검토 필요)`) 해서 신뢰도 차이를 독자가 인지

### 자동 chain 흐름
1. zotero-curate Mode A → KEEP 판정
2. 사용자 `태그 keep` 입력 → Zotero에 `keep/<cat>` write
3. **brief scaffold + fulltext sidecar 동시 fetch** (`--fulltext` 디폴트 ON when PDF 있음):
   - Scaffold → `briefs/quick/{slug}.md` (frontmatter + 빈 5섹션)
   - Fulltext → `.claude/tmp/fulltext/<key>.txt` (sidecar, **git-ignored** — 저작권/저장소 비대 회피)
4. Claude가 sidecar fulltext + abstract를 모두 참조하여 5섹션 채움 → brief.md write
5. 이메일 draft 생성 (Outlook_LLM_Drafter 경로)
6. 사용자 수동 검토 → send

Long-form HTML brief 승격은 별도 수동 작업 (필수 아님).

---

## 4. 디자인 시스템 (Clinical White Editorial · L1)

### 4-1. 컬러 팔레트

| 역할 | HEX | 용도 |
|------|-----|------|
| Background | `#F8F9FC` | 페이지 배경 |
| Ink (Navy) | `#1A2E5A` | 주요 텍스트·구조선 |
| Accent (Sci Red) | `#E8365D` | In Brief, 새 발견 강조 |
| Steel Blue | `#5B8DB8` | 전통 경로(Conventional) |
| Border | `#DDE0ED` | 카드 외곽선 |

### 4-2. 타이포그래피

| 역할 | 폰트 |
|------|------|
| 브랜드 로고 | Syne 800 (Rx) + Crimson Pro 600 Italic (Scriptor) |
| 제목 (Hero) | Crimson Pro Serif 600 |
| 본문 | Pretendard Sans |
| 수치·코드 | DM Mono |

### 4-3. 구조 (5섹션 고정) + Sidebar

Hero → In Brief → Key Findings → Methods → Limitations → Perspective → Sidebar 순서 고정. 섹션별 레이아웃과 Sidebar 필수 항목(수치·별점·모델·태그·배경·리소스·저자)은 기존 long-form brief (`briefs/*.html`)를 canonical 예시로 그대로 따름 — §3a의 quick brief가 canonical 예시를 참조하는 방식과 동일.

---

## 5. 인포그래픽 표준

### 5-1. 사양
- 크기: **16:9 (1600×900)**
- 생성: **ChatGPT Image** (SVG/Figma 금지 — 품질 미달)
- 포맷: PNG, 파일명 `{slug}.png`

### 5-2. 스타일

| 요소 | 규칙 |
|------|------|
| 배경 | `#F8F9FC` |
| 구성 | 2-panel comparison (좌 Steel Blue 전통 / 우 Sci Red 새 발견) |
| 아이콘 | Flat line-art (3D/photo 금지) |
| 제목 | 이미지에 포함 **금지** (HTML에서 표시) |
| 하단 | 빨간 테두리 핵심 요약 박스 1개 |

### 5-3. ChatGPT Image 프롬프트 템플릿

```
Scientific editorial infographic, 16:9, 1600x900, clean flat line-art.

Background: off-white #F8F9FC
Left panel (Steel Blue #5B8DB8): <전통 경로>
Right panel (Scientific Red #E8365D): <새 발견>
Vertical dashed divider between panels.

Left shows: <요소들>
Right shows: <요소들>

Bottom: single red-outlined box
"<한 줄 요약>"

No 3D, no photos, no gradients, no title text in image.
Labels only where necessary (DM Mono style).
```

---

## 6. 대시보드 등록 (index.html)

브리핑 작성 후 반드시 등록. 필드 구성(제목·저널·연도·DOI·URL 2종·태그·핵심 기여 3 bullet·별점)은 `index.html`의 기존 entry를 그대로 따름.

### 태그 원칙

- **primary** (1개): `vaccine`, `DDS`, `immunology`, `delivery`, `oncology` 등
- **secondary** (0-3개): `mRNA`, `LNP`, `cross-presentation`, `clinical` 등

---

## 7. 표준 작업 플로우 (한 줄 호출)

### 트리거
```
"이 논문으로 RxScriptor 브리핑 작성해줘"
"literature brief for <author> et al."
"<author> et al. <year> 논문 브리핑"
```

### Claude 수행 순서
1. 논문 핵심 파악 (PDF 또는 DOI)
2. 슬러그 결정
3. 5섹션 내용 구성
4. Sidebar 정보 추출
5. **HTML 생성** (`briefs/{slug}.html`)
6. 인포그래픽 프롬프트 제공 (사용자가 ChatGPT Image에 입력)
7. 대시보드 등록 정보 정리

### 금지사항
- SVG 인포그래픽 생성 시도
- 슬러그 규칙 무시
- 5섹션 구조 변경
- Clinical White Editorial 외 디자인
- 이미지에 제목 텍스트 포함

---

## 8. 큐레이션 기준 (Tier 2 포트폴리오로서)

이 repo는 **엄선된 논문만** 올림. 기준:
- [ ] DDS·제약 R&D에 기술적 가치
- [ ] 박준영님 전문 관점에서 해석 여지 있음
- [ ] 포트폴리오로서 전문성 보여줄 수 있음
- [ ] Perspective 섹션을 쓸 만한 내용 있음

기준 미달 논문은 rxscriptor-literature에서 수집·요약만 하고 여기 올리지 않음.

---

## 9. 현재 등록 브리핑

Canonical 목록 = `briefs/` (long-form HTML) + `briefs/quick/` (Markdown). `jo-mrna-cd8-2026`, `lnpdb-2026` 2종만 v1 grandfathered 슬러그.

---

## 10. 관련 repo

| Repo | 관계 |
|------|------|
| RxScriptor (Root) | 이 repo 링크 (포트폴리오 허브) |
| rxscriptor-literature | **Tier 1 수집** — 여기서 선별된 것만 이 repo로 |
| rxscriptor-research | 내부 연구 포털. Quarto 연동 검토 가능 |
| rxscriptor-gcbp-design | 회사 디자인 (이 repo는 Clinical White만) |

