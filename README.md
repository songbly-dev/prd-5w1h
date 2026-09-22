# skills

팀 공용 AI 에이전트 스킬 모음입니다. [skills CLI](https://skills.sh)(`npx skills`) 규약을 따르며, Claude Code·Codex·Cursor 등 SKILL.md를 읽는 모든 에이전트에서 쓸 수 있습니다.

## 설치

```bash
# 리포 안 스킬을 골라서 설치
npx skills add songbly-dev/skills

# 특정 스킬만 바로 설치
npx skills add songbly-dev/skills@prd-5w1h
```

- 이 리포는 **private**입니다. 설치하려는 사람이 이 리포 읽기 권한과 `gh auth login`(또는 SSH 키)이 있어야 합니다 — CLI가 내부적으로 `gh repo clone`/`git clone`을 씁니다.
- 권한이 없는 사람에게 줄 때는 리포를 public으로 바꾸거나, 아래 수동 설치를 안내하세요.

### 수동 설치 (CLI 없이)

```bash
git clone https://github.com/songbly-dev/skills.git
# 전역 설치
cp -r skills/skills/prd-5w1h ~/.agents/skills/
# 또는 특정 프로젝트에만
cp -r skills/skills/prd-5w1h <프로젝트>/.agents/skills/
```

## 스킬 목록

| 스킬 | 설명 |
|---|---|
| [`prd-5w1h`](skills/prd-5w1h/SKILL.md) | 5W1H(Why·Who·What·When·Where·How) 입력으로 서비스 기획서 초안 `PRD.md`를 만든다 |

## 새 스킬 추가하기

1. `skills/<스킬이름>/SKILL.md` 파일을 만든다.
2. frontmatter에 `name`과 `description`을 적는다(기존 스킬 참고).
3. 이 README의 스킬 목록 표에 한 줄 추가한다.
4. main에 머지되면 바로 `npx skills add`로 설치된다.
