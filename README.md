# interview-prep

직종과 경험 수준에 맞춘 실전 모의면접 [Claude Code](https://docs.claude.com/en/docs/claude-code) 스킬입니다.
점수 없이 서술형 피드백을 주고, 필요한 답변을 다시 연습하게 돕습니다.

## 특징

- **직종과 경험 수준만 있으면 시작합니다.** 공고·이력서·자소서·포트폴리오는 선택입니다.
- **회사명이 있으면 자동으로 조사합니다.** 공식 채용 안내와 회사 자료를 우선하고, 면접 후기는 참고로만 씁니다.
- **한 번에 질문 하나씩** 묻습니다. 확인할 역량에 따라 질의응답·역할극·자료 리뷰·가상 상황 질문을 고릅니다.
- **점수·등급·합격 판정이 없습니다.** 면접이 끝난 뒤 실제 답변을 근거로 잘한 점과 보완할 점을 설명하고, 재연습을 진행합니다.
- 지원자의 경험이나 수치를 지어내지 않고, 확인하지 못한 회사 정보를 추측하지 않습니다.

## 설치

개인 스킬 폴더에 clone합니다.

macOS / Linux

```bash
git clone https://github.com/bacgam/interview-prep.git ~/.claude/skills/interview-prep
```

Windows (PowerShell)

```powershell
git clone https://github.com/bacgam/interview-prep.git "$env:USERPROFILE\.claude\skills\interview-prep"
```

특정 프로젝트에서만 쓰려면 그 프로젝트의 `.claude/skills/interview-prep`에 clone하면 됩니다.

## 사용법

Claude Code에서 슬래시 명령으로 부르거나, 모의면접을 하고 싶다고 말하면 됩니다.

```
/interview-prep 첫 편의점 아르바이트
/interview-prep 경력 3년 회계직, 지원 회사는 ○○
모의면접 하고 싶어
```

목표 직종이나 경험 수준이 빠져 있으면 그것만 짧게 물어본 뒤 바로 첫 질문을 합니다.
면접 중에는 힌트·일시정지·건너뛰기·종료를 요청할 수 있습니다.

## 파일 구성

| 파일 | 내용 |
|---|---|
| `SKILL.md` | 전체 흐름: 최소 정보 확인 → 회사 조사 → 질문 설계 → 첫 질문 |
| `references/mock.md` | 실전 진행, 꼬리질문, 역할극·자료 리뷰, 종료 후 피드백, 재연습 |
| `references/research.md` | 회사 정보와 면접 후기 조사, 근거 구분 기준 |
| `PROMPT.md` | Claude Code 없이 쓰는 붙여넣기용 프롬프트 |

## Claude Code 없이 쓰기

ChatGPT·Claude.ai·Gemini 같은 일반 챗봇에서는 [PROMPT.md](PROMPT.md)의 프롬프트를 붙여넣어 같은 방식으로 연습할 수 있습니다.
회사 자동 조사는 웹 검색이 켜진 챗봇에서만 동작합니다.

## 출처와 라이선스

이 스킬은 [techeer-sv/Career-Skills](https://github.com/techeer-sv/Career-Skills)
(`skills/hiring-prep-interview`, `skills/hiring-sim-interview`, `skills/hiring-common`,
commit `9a5d83c5d5176cf0f0918a543f443dbac2f67150`)를 각색했습니다.

주요 변경 사항

- 개발 직군 중심에서 모든 직종을 다루는 모의면접 스킬 하나로 통합
- 사전 정보를 직종과 경험 수준으로 최소화하고, 지원자 자료는 선택으로 변경
- 회사명이 있으면 자동 조사, 역할극과 자료 리뷰 추가
- 점수와 준비 문서 모드를 없애고, 서술형 피드백과 재연습 중심으로 변경

[MIT License](LICENSE)
