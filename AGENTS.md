# skills_repo — Claude Code 스킬 3종 (원본 보관소)

`ai-readiness-cartography`(repo AI-준비도 채점+HTML 대시보드) · `improve-token-efficiency`(세션 로그 → 토큰·비용 리포트) · `presentation_slides`(대본 → 발표용 HTML 슬라이드).

## ★ 이 폴더는 원본이다 — 실제로 도는 건 설치본이다

| | 위치 |
|---|---|
| 원본(이 repo) | `E:\dev\skills_repo` |
| **설치본(실행되는 것)** | `~/.claude/skills/` → `OneDrive/claude-sync/skills` (심볼릭 링크) |

⚠️ **여기만 고치면 동작이 하나도 안 바뀐다.** AI가 부르는 건 설치본이다.
⚠️ 반대로 **설치본만 고치면 git 이력에 안 남는다**(OneDrive 는 버전관리가 아니다).
→ 스킬 내용을 고칠 땐 **양쪽 다** 고칠 것.

## 설치 방법

```bash
cp -r <스킬폴더> ~/.claude/skills/
rm -rf ~/.claude/skills/<스킬폴더>/scripts/__pycache__
```

`__pycache__`(파이썬 컴파일 캐시)는 옮기지 않는다. 새 세션부터 스킬 목록에 뜬다.

- **2026-08-14: 3종 전부 설치 완료.** 그전까지는 이 폴더에 파일만 있고 설치가 안 돼 있어서 **스킬이 아예 안 불렸다**(쓰는 기능인 줄 알았는데 호출되지 않던 상태).
- OneDrive 동기 폴더라 한 번 넣으면 노트북에도 따라온다.

## 주의

- ⚠️ **Windows 실행 버그·경로 오탐 이력이 있다** — 2026-07-02 커밋 2건이 그 수정이다(`.tsx`/`.json` 경로를 잘라 없는 파일로 지어내던 결함, 비용 라벨 오표기). 스킬 결과가 이상하면 이 계열을 먼저 의심할 것.
- upstream 원격이 없다(`origin` = `hyunn0923/skills_repo` 하나). 최초 커밋만 외부(Jae Ha, 맥)이고 이후 수정은 우리 것이라, **받아올 원본이 없다 = 여기가 정본**이다.
