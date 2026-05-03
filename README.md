# 🧽 OS Interview Skill

> **인터뷰 한 바퀴 → 당신의 OS 청사진 + 첫 부품 1개.** 손에 들고 즉시 사용 가능.

40~60분 인터뷰가 끝나면 두 파일이 손에 남습니다:

1. `os-blueprint.md` — 당신만의 OS 청사진 (선언문 · 통점 · 이상향 · 부품 후보 리스트)
2. **첫 부품 결과물 1파일** — 본인이 선택한 형태로:

| 형태 | 출력 파일 | 설치 위치 | 인터뷰 끝 → 사용까지 |
|---|---|---|---|
| **A. Claude 스킬** | `<이름>.skill.md` | `~/.claude/skills/` | **즉시** |
| **B. Claude Code 플러그인** | `<이름>/` 폴더 | `~/.claude/plugins/` | **즉시** |
| **C. 독립 프로덕트 PRD** | `<이름>.prd.md` | (Claude Code에 던짐) | 한 단계 더 (코드 생성) |

A·B는 인터뷰 끝나는 그 순간부터 사용 가능 — OS의 첫 부품이 그날 등록됩니다.

---

## OS가 뭔가요

**OS** = 당신이 매일 켜서 자기 일과 삶을 운용하는 시스템. 부품 하나하나가 모여 한 사람의 OS가 됩니다.

> 모두에게 같은 OS는 없습니다. 마케터의 OS와 1인 대표의 OS는 다르게 생겨야 정상이에요. 이 스킬은 **여러분의 OS의 첫 부품**을 함께 끌어내줍니다.

---

## 빠른 시작 (3분 설치)

### 1. Clone

```bash
git clone https://github.com/selfishclub/os-interview-skill.git
cd os-interview-skill
```

### 2. 메인 스킬을 전역 설치

```bash
mkdir -p ~/.claude/skills/os-interview
cp SKILL.md ~/.claude/skills/os-interview/
cp -r templates ~/.claude/skills/os-interview/
```

> 💡 **심볼릭 링크 (추천)**: 위 cp 대신 `ln -s` 를 쓰면 GitHub에서 업데이트한 게 자동 반영돼요.
> ```bash
> ln -s "$(pwd)" ~/.claude/skills/os-interview
> ```

### 3. 발동

어떤 폴더에서든 Claude Code (또는 Claude Desktop)를 켜고, 다음 같은 메시지를 던지면 자동 발동됩니다:

> "내 OS 만들고 싶어"
> "나만의 워크플로우 시스템 짜고 싶어"
> "내가 매일 쓸 도구 하나 만들어보자"

40~60분 후 손에 두 파일이 남아있을 거예요.

---

## 인터뷰는 어떻게 흐르나요

```
Phase 1 · OS 전체 청사진 (Step 1~4) — 30~40분 · 톤: 사고 파트너
  Step 1. 풍경      — 지금 어떤 일/삶을 살고 있는가
  Step 2. 통점      — 반복되는 짜증·낭비·막힘
  Step 3. 이상향    — 그게 풀린 모습 (= 내 OS 선언문) ⭐
  Step 4. 부품 매핑 — 도구 후보 3~7개

Phase 2 · 첫 부품 + 형태 선택 (Step 5) — 5분 · 톤 전환
  Step 5. 후보 중 1개 결정 + 형태(A/B/C) 선택

Phase 3 · 형태별 결과물 1파일 (Step 6) — 10~15분 · 톤: 발판형
  Step 6. 선택한 템플릿에 따라 빠른 질문 → 결과물 한 파일
```

**Phase 1의 톤이 핵심**입니다. Claude는 단순 질문 봇이 아니라 **가설을 던지고 검증받는 사고 파트너**로 동작해요. 사용자가 본인도 몰랐던 통점·이상향을 발견하게 됩니다.

---

## 무엇이 들어있나

```
os-interview-skill/
├── README.md               # 이 파일
├── SKILL.md                # ← 인터뷰 스킬 본체. 키트의 핵심
├── templates/
│   ├── output-skill.md     # Step 6 분기 A — 스킬 출력 양식
│   ├── output-plugin.md    # Step 6 분기 B — 플러그인 출력 양식
│   └── output-prd.md       # Step 6 분기 C — PRD 출력 양식
├── examples/
│   └── content-creator-weekly-review/
│       ├── os-blueprint.md
│       └── weekly-content-review.skill.md
└── LICENSE
```

---

## 누구를 위한 건가

- 매일 Claude를 켜는데 "어떻게 더 잘 굴릴 수 있을까"가 답답한 사람
- 자기만의 시스템을 만들고 싶지만 막연한 사람
- "있으면 좋겠다"는 도구 아이디어가 머릿속에 있지만 실행으로 못 옮기는 사람
- **셀피쉬클럽 스폰지클럽 1기 크루** (이 키트의 첫 청자)

---

## 자주 묻는 질문

**Q. 이 스킬을 한 사람이 여러 번 쓸 수 있나요?**
네, 권장합니다. 첫 인터뷰에서 OS 청사진 + 첫 부품이 나오고, 그 부품을 사용해본 뒤 두 번째 인터뷰로 다음 부품을 만드세요. 두 번째부터는 Phase 1을 짧게 갈 수 있습니다 (이미 청사진이 있으니).

**Q. 결과물이 사람마다 천차만별일 텐데, 그게 의도인가요?**
네. 같은 답이 나오면 그건 인터뷰가 아니라 설문조사예요. 키트가 표준화하는 건 답이 아니라 **단계와 톤**입니다. 다양성이 가치.

**Q. A/B/C를 잘못 골라도 되나요?**
인터뷰 도중 형태를 바꿔도 됩니다. Step 5에서 A로 시작했는데 답하다 보니 B가 맞다 싶으면 Claude에게 "사실 B로 가야 할 것 같아"라고 하세요.

**Q. Claude Desktop과 Claude Code 둘 다에서 동작하나요?**
네. 둘 다 `~/.claude/skills/` 를 읽어요. Claude Desktop의 정확한 스킬 등록 절차는 https://docs.claude.com → "Skills" 참고.

---

## 라이센스 / 출처

[MIT License](./LICENSE). 셀피쉬클럽 스폰지클럽 1기의 작업물에서 출발. 자유롭게 fork·수정·재배포 가능.

본인의 인터뷰 결과(`os-blueprint.md` + 첫 부품)를 [`examples/`](./examples) 에 PR로 올려주시면 다른 사람의 첫 영감이 됩니다.

> 냅다 흡수하고 · 냅다 만들고 · 냅다 세상에 내놓는다 🧽
