# 김태인 | Taein Kim

TypeScript·React로 사용자 화면을 만들고, Python 서버·데이터·AI 기능을 연결합니다.
입력한 요청과 실제 처리 결과가 화면에서 어떻게 전달되는지 살피며 개발합니다.

## 주요 프로젝트

| 프로젝트 | 서비스와 담당 작업 | 기술 |
| --- | --- | --- |
| [안전골목](https://github.com/taein0926/SafeAlley) | 보행 조건에 맞는 경로 추천. 공간정보 처리, AI 기능 구현·연동, 서버·지도 화면 연결과 배포 확인 | TypeScript, React, CesiumJS, Python, FastAPI, PostGIS |
| [PinUp](projects/pinup/README.md) | 지도 기반 맛집 리뷰 팀 프로젝트. 검색바·가게 카드·이미지 슬라이더, 목록/리뷰 화면 전환과 리뷰 반영 | TypeScript, React, styled-components |
| [AI 페르소나](https://github.com/taein0926/ai-persona) | 화재 대피 시뮬레이션 PoC. 기존 엔진에 개인별 LLM 판단을 연결하고 판단·이동 결과를 기록·표시 | Python, Ollama, JavaScript, Docker |
| [집밥코인](https://github.com/24-1-LikePotato/Zipbap-Coin-FE) | 식재료 관리·레시피 팀 프로젝트. 등록 입력 검사, API 응답 처리와 레시피 상세 화면 | JavaScript, React, Axios |

AI 페르소나는 개발 중인 PoC이며 [공개 화면](https://taein0926.github.io/ai-persona/)에서는 저장된 결과를 재생할 수 있습니다.
팀 프로젝트의 담당 범위와 관련 PR은 각 소개 문서에서 확인할 수 있습니다.

## 개발할 때 살피는 부분

- **입력과 결과의 구분**: 안전골목의 입력 미리보기와 실제 계산 조건, AI 페르소나의 모델 제안과 실제 이동 결과를 나누어 표시했습니다.
- **실패와 기존 정보 보존**: 모델 응답 검사·개별 요청 실패 처리, 배포 전후 데이터·설정 보존을 확인했습니다.
- **리뷰와 화면 기준**: PinUp에서 상태 타입에 대한 리뷰를 반영하고 기존 글꼴·간격 기준을 적용했습니다.

## 사용 경험

- 화면: TypeScript, JavaScript, React, styled-components, CesiumJS
- 서버·데이터: Python, FastAPI, PostgreSQL/PostGIS
- 개발 환경: Git/GitHub, Docker
- AI 개발 도구: 안전골목·AI 페르소나 개발에 Codex, CS Wiki 개발에 Gemini CLI 활용

## 다른 작업

[CS Wiki](https://github.com/taein0926/cs-llm-wiki)는 원문을 Markdown 문서로 생성·저장하고 기존 사용자 메모를 보존하는 개인 도구입니다. 문서 생성 파이프라인과 Streamlit 문서 탐색 화면을 구현했으며, 채팅·CVE 검색 시연과 실제 구현의 범위는 README에 구분했습니다.

## 연락처

[kimtaein0926@gmail.com](mailto:kimtaein0926@gmail.com)
