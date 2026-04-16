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

## 2. 디렉토리 구조 (유지)

```
literature-archive/
├── CLAUDE.md                           이 파일
├── README.md
├── index.html                          대시보드 (검색·필터)
│
├── briefs/
│   ├── jo-mrna-cd8-2026.html          슬러그: {firstauthor}-{topic}-{year}
│   └── ...
│
└── assets/
    ├── infographic/
    │   ├── jo-mrna-cd8-2026.png       16:9, Hero + 썸네일 겸용
    │   └── ...
    └── (공통 CSS/폰트, 있다면)
```

---

## 3. 브리핑 작성 표준 (절대 준수)

### 3-1. 슬러그 규칙

```
{firstauthor}-{topic}-{year}
```

**예시**:
- Jo et al. 2026, mRNA CD8 → `jo-mrna-cd8-2026`
- Lobb et al. 2026, i.v. LNP → `lobb-ivlnp-2026`

**규칙**: 성 소문자, topic 1-2단어 하이픈 구분, year 4자리, 전부 소문자

### 3-2. 파일 배치

```
briefs/{slug}.html                      브리핑 페이지
assets/infographic/{slug}.png           인포그래픽 (Hero + 썸네일)
```

SVG 초안, preview 파일은 로컬 임시 폴더만 (repo에 커밋 금지)

### 3-3. Git 커밋 메시지

```
Add: {topic} brief ({primary-tag})
```

예: `Add: mRNA-CD8 priming brief (vaccine)`

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

### 4-3. 구조 (5섹션 고정)

```
Hero (magazine spread — 좌 텍스트 / 우 인포그래픽)
  ↓
In Brief (빨간 좌측 라인, 5포인트)
  ↓
§ I. Key Findings (카드 3-5개)
  ↓
§ II. Methods Overview (4-box)
  ↓
§ III. Limitations (red box, 3-5)
  ↓
§ IV. Perspective (DDS 관점, accent box, 3-4)
  ↓
Sidebar (수치/별점/모델/태그/배경/리소스/저자)
```

### 4-4. Sidebar 필수 항목

- 수치 (Subjects, Cell count)
- 별점 (1~5★, 미평가 가능)
- 모델 (mouse, human)
- 태그 (primary + secondary)
- 배경 (Background 한 줄)
- 리소스 (GEO, code)
- 저자 (1st + corresponding)

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

브리핑 작성 후 반드시 등록:

| 필드 | 값 |
|------|-----|
| 제목 | 논문 full title (영문) |
| 저널 | Nature, Cell 등 |
| 발행연도 | 4자리 |
| DOI | `10.xxxx/xxxxx` |
| 브리핑 URL | `./briefs/{slug}.html` |
| 이미지 URL | `./assets/infographic/{slug}.png` |
| 태그 | primary 먼저, secondary 추가 |
| 핵심 기여 | 3개 bullet |
| 별점 | 1~5 (미평가 가능) |

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

| 슬러그 | 논문 | 발행 | 별점 |
|--------|------|------|------|
| `jo-mrna-cd8-2026` | Jo et al., mRNA vaccines & CD8 priming (Nature) | 2026 | 미평가 |

(새 브리핑 추가 시 갱신)

---

## 10. 관련 repo

| Repo | 관계 |
|------|------|
| RxScriptor (Root) | 이 repo 링크 (포트폴리오 허브) |
| rxscriptor-literature | **Tier 1 수집** — 여기서 선별된 것만 이 repo로 |
| rxscriptor-research | 내부 연구 포털. Quarto 연동 검토 가능 |
| rxscriptor-gcbp-design | 회사 디자인 (이 repo는 Clinical White만) |

---

## 11. 변경 이력

| 날짜 | 변경 |
|------|------|
| 2026-04-16 | 초기 작성. Jo et al. 2026 브리핑 작업에서 정립된 L1 표준 반영 |
