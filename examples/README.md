# 예시 스킬 모음

이 폴더는 [`GUIDE.md`](../GUIDE.md)를 따라 만든 인터뷰 스킬의 **참고용 예시**입니다. 본인 스킬을 설계하기 전에 한 번 훑어보세요. "아, 이런 식으로 풀 수 있구나"의 감을 잡는 게 목적입니다.

> ⚠️ **주의**: 이건 영감용 예시일 뿐, 정답이 아닙니다. 본인 업무 맥락은 다르게 생겼어요. **그대로 베끼지 말고**, 구조만 참고해서 본인 답으로 다시 채우세요.

---

## 현재 들어있는 예시

| 폴더 | 누구를 위한가 | 무엇을 만들어내는가 |
|---|---|---|
| [`client-brief-marketer/`](./client-brief-marketer/) | 마케터 — 신규 클라이언트 미팅 직전/직후 | 1페이지 클라이언트 브리프 |

---

## 본인 예시를 추가하고 싶다면

본인의 v0.1을 만든 다음, 이 폴더에 `<본인-스킬-이름>/SKILL.md`로 PR을 보내주세요. 다른 크루의 첫 영감이 될 거예요.

```bash
# fork 뜨고 PR 흐름
gh repo fork <이 repo URL>
cd sponge-interview-skill-kit
mkdir -p examples/<your-skill-name>
cp ~/Documents/my-interview-skill/SKILL.md examples/<your-skill-name>/
git checkout -b add-<your-skill-name>
git add examples/<your-skill-name>
git commit -m "add example: <your skill name>"
git push origin add-<your-skill-name>
gh pr create
```
