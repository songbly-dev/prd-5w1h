# prd-5w1h

[![skills.sh](https://skills.sh/b/songbly-dev/prd-5w1h)](https://skills.sh/songbly-dev/prd-5w1h)

5W1H(Why·Who·What·When·Where·How) 입력으로 서비스 기획서 초안 `PRD.md`를 만드는 AI 에이전트 스킬입니다. Claude Code·Codex·Cursor 등 SKILL.md를 읽는 모든 에이전트에서 쓸 수 있습니다.

## 설치

```bash
npx skills add songbly-dev/prd-5w1h
```

Node.js만 설치돼 있으면 위 명령 한 줄로 끝납니다(별도 회원가입·로그인 불필요).

### 수동 설치 (CLI 없이)

```bash
git clone https://github.com/songbly-dev/prd-5w1h.git
# 전역 설치
mkdir -p ~/.agents/skills/prd-5w1h && cp prd-5w1h/SKILL.md ~/.agents/skills/prd-5w1h/
# 또는 특정 프로젝트에만
mkdir -p <프로젝트>/.agents/skills/prd-5w1h && cp prd-5w1h/SKILL.md <프로젝트>/.agents/skills/prd-5w1h/
```

## 사용법

설치 후 에이전트에게 아래처럼 요청하면 동작합니다.

- "PRD 써줘", "기획서 초안 만들어줘", "5w1h 기획서", `/prd-5w1h`
- 서비스명과 5W1H(왜·누구·무엇·언제·어디서·어떻게)를 함께 주면 바로 초안을 뽑고, 정보가 없으면 입력 양식을 보여줍니다.
- 결과물은 프로젝트 루트의 `PRD.md` — 「이 문서에 대하여」+ 목차 + 본문 5섹션(개요·페르소나·주요 기능·페이지 구조·성공 지표) 고정 포맷입니다.

## 스킬 파일

- [`SKILL.md`](SKILL.md) — 스킬 본체(입력 계약·절차·출력 포맷·금지 규칙)
