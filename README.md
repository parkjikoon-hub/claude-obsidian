# Claude Obsidian

Obsidian 안에서 Claude AI와 대화하고, 노트를 분석·저장하는 KNOT 플러그인입니다.

![version](https://img.shields.io/badge/version-1.1.0-blue)
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
| 💬 **Claude 채팅 사이드바** | Obsidian 오른쪽 패널에서 Claude AI와 실시간 대화 |
| 🗺️ **Memory Map** | BM25 알고리즘으로 관련 노트를 로컬에서 탐색 (API 비용 0원) |
| 📌 **핀 노트 영구 저장** | 재시작 후에도 핀 고정 노트 유지 |
| ⚡ **슬래시(/) 커맨드** | `/요약` `/분석` `/기획서` 등 입력창에서 빠른 명령 실행 |
| ⏱️ **작업 타임라인** | AI 응답 중 진행 단계 실시간 표시 |
| 📎 **노트 컨텍스트 자동 전달** | 현재 열린 노트를 Claude에게 자동 전달 |
| 💾 **노트 자동 생성** | 대화 내용을 KNOT 프론트매터가 포함된 노트로 저장 |
| 🧠 **Extended Thinking** | Low / Medium / High / Max 사고 단계 선택 |

---

## 슬래시(/) 커맨드 목록

입력창에 `/`를 입력하면 커맨드 메뉴가 열립니다.

| 커맨드 | 동작 |
|--------|------|
| `/요약` | 현재 노트 핵심 요약 |
| `/분석` | 깊이 있는 분석 + 인사이트 |
| `/기획서` | 대화를 기획서 형식으로 변환 |
| `/회의록` | 대화를 회의록으로 정리 |
| `/액션` | 할 일 체크리스트 추출 |
| `/저장` | 대화를 옵시디언 노트로 저장 |
| `/번역` | 현재 노트 한→영 번역 |
| `/초기화` | 대화 초기화 |

---

## Memory Map 사용법

1. 패널 상단 **"구축하기"** 클릭 → 볼트 전체 노트 색인 생성
2. 노트를 열고 **"관련 노트 찾기"** 클릭 → 관련 노트 최대 8개 추천
3. 추천 결과의 📌 버튼으로 바로 핀 고정 가능
4. **"재구축"** 으로 새 노트 추가 후 색인 갱신

> Memory Map은 완전히 로컬에서 동작합니다. API 호출 없이 무료로 사용할 수 있습니다.

---

## 사전 준비

### Claude API 키 발급

1. [Anthropic Console](https://console.anthropic.com/settings/keys) 접속
2. **"Create Key"** 클릭 후 키 복사 (`sk-ant-...` 형태)

---

## 설치 방법

### 직접 설치 (권장)

1. 이 저장소에서 파일 3개 다운로드:
   - `main.js`
   - `manifest.json`
   - `styles.css`

2. 옵시디언 볼트 폴더에 복사:
   ```
   <볼트 경로>/.obsidian/plugins/claude-obsidian/
   ```

3. 옵시디언 재시작 → **설정 → 커뮤니티 플러그인 → Claude Obsidian** 활성화

4. **설정 → Claude Obsidian → API 키** 입력

### Git 클론으로 설치

```bash
cd <볼트 경로>/.obsidian/plugins/
git clone https://github.com/parkjikoon-hub/claude-obsidian
```

---

## 사용 방법

### 패널 열기
- 왼쪽 사이드바의 **🤖 아이콘** 클릭
- 또는 `Ctrl+P` → `Claude Obsidian 패널 열기`

### 메시지 전송
- `Enter`: 메시지 전송
- `Shift+Enter` / `Ctrl+Enter`: 줄바꿈
- `/`: 슬래시 커맨드 메뉴 열기

### 노트 자동 저장
채팅창에서 다음 키워드를 포함하면 자동으로 노트가 생성됩니다:
- "저장해줘", "노트로 저장", "파일로 만들어", "기획서로", "회의록으로"

---

## 지원 모델

| 모델 | 특징 |
|------|------|
| Claude Sonnet 4.6 | 균형 잡힌 성능 (추천) |
| Claude Opus 4.6 | 고성능 |
| Claude Opus 4.7 | 최고 성능 |

---

## KNOT 플러그인 생태계

| 플러그인 | AI | 저장소 |
|----------|-----|--------|
| **Claude Obsidian** | Anthropic Claude | [parkjikoon-hub/claude-obsidian](https://github.com/parkjikoon-hub/claude-obsidian) |
| **Gemini Obsidian** | Google Gemini | [parkjikoon-hub/gemini-obsidian](https://github.com/parkjikoon-hub/gemini-obsidian) |
| **Codex Obsidian** | OpenAI GPT | [parkjikoon-hub/codex-obsidian](https://github.com/parkjikoon-hub/codex-obsidian) |

---

## 개인정보 보호

- API 키는 옵시디언 로컬 설정에만 저장됩니다.
- 대화 내용은 Anthropic API로만 전송됩니다.
- Memory Map 색인은 볼트 내 로컬 파일(`.claude-obsidian/memory/`)에 저장됩니다.

---

## 라이선스

MIT License

---

Made with ❤️ by [KNOT](https://github.com/parkjikoon-hub)
