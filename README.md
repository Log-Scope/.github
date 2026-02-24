# .github
# 🚀 Organization Git 협업 가이드

이 레포지토리(`.github`)는 우리 Organization의 **기본 Issue/PR 템플릿**과 협업 규칙(표준)을 관리합니다.  
모든 프로젝트 레포지토리는 아래 규칙에 따라 **브랜치 → PR → 리뷰 → 머지** 흐름으로 진행합니다.


## 1) 기본 원칙

### Default Branch
- 기본 브랜치: **`main`**

### main 브랜치 보호 규칙
- `main`에는 **직접 push 금지**
- `main` 반영은 **Pull Request(PR)로만** 가능
- PR은 **승인 1명 필수**
- PR 내 리뷰 코멘트/대화는 **Resolve(해결) 후** 머지 가능


## 2) 이슈(Issue) 사용 규칙

이슈는 다음 중 하나로 작성합니다.
- **Feature**: 기능 추가/변경
- **Bug**: 버그 제보/수정
- **Blank**: 논의/메모/조사 등 자유 이슈

**권장 흐름**
1. 작업 시작 전 **이슈를 먼저 생성**
2. 이슈 번호를 기준으로 브랜치 생성
3. PR에서 이슈를 연결해 **머지 시 자동 종료**


## 3) 브랜치 네이밍 규칙 (권장)

이슈 번호를 포함해 브랜치명을 통일합니다.
- `feat/<이슈번호>-요약`
- `fix/<이슈번호>-요약`
- `chore/<이슈번호>-요약`
- `docs/<이슈번호>-요약`

**예시**
- `feat/12-queue-eta`
- `fix/34-payment-dup`
- `chore/7-config-cleanup`


## 4) PR 규칙

### PR 제목 규칙 (필수)
PR 제목은 아래 형식으로 작성합니다.

> `feat|fix|chore|docs: 요약 (#이슈번호)`

- 예시: `feat: 대기열 ETA 표시 (#12)`

### PR 본문 규칙 (필수)
PR 본문에 아래 문구를 포함하여 이슈를 연결합니다.

> `Closes #<이슈번호>`

- 예시: `Closes #12`


## 5) 이슈 자동 종료(Auto-close) 규칙 (필수)

PR이 **머지(merge)** 될 때 이슈가 자동으로 닫히려면,  
**PR 본문(Description)** 에 아래 키워드 중 하나를 **이슈 번호와 함께** 포함해야 합니다.

### 자동 종료 키워드
- `close`, `closes`, `closed`
- `fix`, `fixes`, `fixed`
- `resolve`, `resolves`, `resolved`

### 사용 예시 (권장: Closes)
- `Closes #12`
- `Fixes #34`
- `Resolves #7`

### 여러 이슈를 한 번에 닫기
- `Closes #12, #13`
또는
- `Closes #12`
- `Closes #13`

### 주의
- **이 문구는 반드시 PR 본문에 있어야 함** (커밋 메시지/코멘트에만 있으면 실수 가능)
- 자동 종료는 **PR이 기본 브랜치(main)에 머지될 때** 동작하는 게 원칙
- “참고용 링크”로만 달면 자동 종료가 안 되므로, 반드시 위 키워드로 연결


## 6) 커밋 메시지 규칙 (권장)

권장 커밋 메시지 형식:
> `feat|fix|chore|docs: 요약 (#이슈번호)`

예시:
```bash
git commit -m "feat: 대기열 ETA API 추가 (#12)"
