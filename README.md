# Claude Obsidian

Obsidian 안에서 Claude AI와 대화하고, 대화 내용을 자동으로 노트로 생성하는 플러그인입니다.

![version](https://img.shields.io/badge/version-1.4.19-blue)
![obsidian](https://img.shields.io/badge/Obsidian-1.0.0+-purple)
![license](https://img.shields.io/badge/license-MIT-green)

---

## KNOT란?

> **K**now · **N**ote · **O**utput · **T**ransform

지식을 **알고(Know)** → **기록하고(Note)** → **산출하고(Output)** → **변환한다(Transform)**

KNOT는 단순한 노트 도구가 아닌, 지식이 행동으로 이어지는 흐름을 만드는 플러그인 생태계입니다.
매듭(Knot)처럼 흩어진 생각과 대화를 단단하게 엮어 하나의 지식으로 만들어줍니다.

---

## 주요 기능

| 기능 | 설명 |
|------|------|
| 💬 **Claude 채팅 사이드바** | Obsidian 안에서 Claude AI와 실시간 대화 |
| 📎 **노트 컨텍스트 자동 전달** | 현재 열린 노트를 Claude에게 자동 전달 |
| 💾 **노트 자동 생성** | 대화 내용을 KNOT 프론트매터가 포함된 노트로 저장 |
| ⚙️ **파일 작업** | 파일 읽기·쓰기·실행 등 에이전트 기능 |

---

## 사전 준비

Claude Code CLI가 설치되어 있어야 합니다.

```bash
# 설치 확인
claude --version

# 설치 (없을 경우)
npm install -g @anthropic-ai/claude-code
```

---

## 설치 방법

1. 이 저장소에서 파일 3개 다운로드:
   - `main.js`
   - `manifest.json`
   - `styles.css`

2. 옵시디언 볼트 폴더에 복사:
   ```
   <볼트 경로>/.obsidian/plugins/claude-obsidian/
   ```

3. 옵시디언 재시작 → **설정 → 커뮤니티 플러그인 → Claude Obsidian** 활성화

### Git 클론으로 설치

```bash
cd <볼트 경로>/.obsidian/plugins/
git clone https://github.com/parkjikoon-hub/claude-obsidian
```

---

## KNOT 플러그인 생태계

| 플러그인 | AI | 저장소 |
|----------|-----|--------|
| **Claude Obsidian** | Anthropic Claude | [parkjikoon-hub/claude-obsidian](https://github.com/parkjikoon-hub/claude-obsidian) |
| **Gemini Obsidian** | Google Gemini | [parkjikoon-hub/gemini-obsidian](https://github.com/parkjikoon-hub/gemini-obsidian) |
| **Codex Obsidian** | OpenAI Codex | [parkjikoon-hub/codex-obsidian](https://github.com/parkjikoon-hub/codex-obsidian) |

---

## 라이선스

MIT License

---

Made with ❤️ by [KNOT](https://github.com/parkjikoon-hub)
