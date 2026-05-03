# 🧽 Sponge Interview Skill Kit

> 스폰지클럽 1기 크루를 위한 — 나만의 인터뷰 스킬을 처음부터 만들어보는 키트

**셀피쉬클럽이 W1에 배포한 스폰지 인터뷰 스킬**이 모두에게 같은 질문을 던졌다면, 이 키트로 만드는 스킬은 **여러분의 일에서만 나올 수 있는 질문**을 던집니다.

이 키트는 빈 폴더에서 GitHub 업로드까지 한 바퀴를 안내합니다. 한 번 돌리는 데 약 2~3시간.

---

## 누구를 위한 건가

- 스폰지클럽 1기 크루
- W1 인터뷰 스킬을 써보고 "내 업무에는 다른 질문이 필요한데"가 떠오른 사람
- 트랙 A(나만의 AI OS) 또는 트랙 B(유저 프로덕트)를 만들기 전에, 방향을 날카롭게 잡고 싶은 사람

---

## 이 키트에 뭐가 들었나

| 파일/폴더 | 무엇 |
|---|---|
| [`GUIDE.md`](./GUIDE.md) | **메인 가이드** — Step 1~7 전체 흐름 |
| [`worksheet.md`](./worksheet.md) | Step 2 설계 워크시트 (복사해서 본인 답으로 채우기) |
| [`templates/SKILL.md.template`](./templates/SKILL.md.template) | 빈 SKILL.md 템플릿 — Claude Code에게 넘기면 채워줌 |
| [`examples/`](./examples/) | 참고용 예시 스킬 모음 |

---

## 빠른 시작 (3분 버전)

1. 이 repo를 **Fork** 또는 다운로드
2. [`GUIDE.md`](./GUIDE.md) 열고 Step 1부터 순서대로
3. 막히면 [`worksheet.md`](./worksheet.md)부터 채워보기

> 처음이면 **반드시** GUIDE.md를 정독하고 시작하세요. 워크시트를 건너뛰면 Step 4가 헷갈려져요.

---

## 전역(global) 스킬로 설치하기

이 키트로 만든 스킬은 **특정 프로젝트에 갇히지 않고**, 어떤 작업을 하든 항상 호출할 수 있어야 진짜 쓸모가 생겨요. 클라이언트 브리핑이든, 주간 회고든, 콘텐츠 기획이든 — 인터뷰가 필요한 모든 자리에서.

### Claude Code에서 전역으로 쓰기

Claude Code는 두 위치에서 스킬을 찾습니다:

- **전역**: `~/.claude/skills/<스킬이름>/SKILL.md` ← **이 키트는 여기를 권장**
- **프로젝트별**: `<프로젝트>/.claude/skills/<스킬이름>/SKILL.md`

따라서 만든 스킬을 어떤 프로젝트에서든 트리거하려면:

```bash
# 작업했던 폴더를 통째로 전역 skills 폴더로 복사
mkdir -p ~/.claude/skills
cp -r ~/Documents/my-interview-skill ~/.claude/skills/
```

또는 **심볼릭 링크**로 걸어두면 GitHub repo에서 수정한 게 그대로 반영됩니다 (추천):

```bash
mkdir -p ~/.claude/skills
ln -s ~/Documents/my-interview-skill ~/.claude/skills/my-interview-skill
```

이렇게 해두면 어떤 폴더에서 `claude`를 켜도 본인의 인터뷰 스킬이 트리거됩니다.

### Claude Desktop에서 쓰기

Claude Desktop의 스킬 등록 인터페이스는 시점에 따라 달라질 수 있어요. **가장 정확한 절차는 [docs.claude.com](https://docs.claude.com)에서 "Skills"를 검색**해서 확인하세요.

---

## 만든 다음 — #냅다-공유

만든 채로 두면 1주치 학습. #냅다-공유에 던지면 8~10주치가 돌아와요.

```
🧽 [내 이름] · 인터뷰 스킬 v0.1 풀었습니다

[한 줄 소개]
이 스킬은 ___을 인터뷰해서 ___을 만들어내는 스킬이에요.

[GitHub]
https://github.com/내유저네임/my-interview-skill

[지금 막힌 지점]
___
```

다른 크루가 fork 떠서 자기 버전으로 가져가는 게 **이기적 공유의 가장 또렷한 형태** — 하나가 여섯 개로 돌아옵니다.

---

## 라이센스 / 출처

- 이 키트는 **셀피쉬클럽 스폰지클럽 1기**의 작업 결과물에서 출발합니다.
- 자유롭게 fork, 수정, 재배포 가능합니다 ([MIT License](./LICENSE)).
- 본인의 fork에서 더 좋은 흐름을 만들었다면 PR 또는 #냅다-공유로 알려주세요.

> 냅다 흡수하고 · 냅다 만들고 · 냅다 세상에 내놓는다 🧽
