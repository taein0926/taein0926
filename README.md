# 김태인 | Taein Kim

Python으로 서버와 AI 기능을 연결하고, TypeScript와 React로 사용자 화면을 개발합니다. 구현한 기능이 의도대로 동작하는지 테스트와 실험으로 확인합니다.

`kimtaein0926@gmail.com`

## 대표 프로젝트

### 안전골목

보행자가 요청한 조건에 맞춰 인천 미추홀구의 경로를 비교하는 웹 서비스입니다. 자연어·음성 입력을 구현해 추출한 조건을 원문과 대조하고, 경로 계산에 실제 사용한 조건을 지도에 표시했습니다.

[저장소](https://github.com/taein0926/SafeAlley) · [조건 검증](https://github.com/taein0926/SafeAlley/blob/main/docs/natural-language.md) · [VM 배포 검증](https://github.com/taein0926/SafeAlley/blob/main/docs/vm-deployment-2026-11-03.md)

### AI 페르소나 화재 대피 시뮬레이션

지하철역 화재 상황에서 가상 인물의 관측과 판단을 이동에 반영하는 연구용 PoC입니다. 기존 보행 엔진에 로컬 LLM을 연결하고 실행 설정을 조정해, 동일 모델과 입력을 사용한 100명 실험에서 **계산과 저장 시간을 65분 23초에서 46분 45초로 줄였습니다.**

[저장소](https://github.com/taein0926/ai-persona) · [공개 시연](https://taein0926.github.io/ai-persona/) · [GitHub Actions 배포](https://github.com/taein0926/ai-persona/blob/main/.github/workflows/deploy-pages.yml)

### 해안 미세 사람 탐지

해변과 해상 영상에 작게 찍힌 사람을 탐지하기 위해 SSPNet과 YOLO26m을 같은 평가 코드로 비교했습니다. SSPNet을 해변 영상으로 추가 학습한 뒤, **해변 영상의 정밀도는 11.1%에서 70.5%로 올랐고 해상 영상의 재현율은 78.0%에서 64.0%로 내려갔습니다.**

[비교 이미지와 전체 실험 결과](https://github.com/taein0926/coastal-tiny-person-detection)

## 추가 프로젝트

- **C++ AVL Tree Set** — 값 삽입과 균형 처리를 담당하고, 순위 조회의 경계 조건을 Google Test로 확인했습니다.
- **AI CS Wiki** — 학습 자료를 Markdown으로 생성하고, 문서를 다시 생성할 때 기존 사용자 메모를 복원하도록 구현했습니다. [저장소](https://github.com/taein0926/cs-llm-wiki)
- **집밥코인** — 식재료 등록의 입력과 API 응답을 처리하고, 레시피의 재료·조리 순서·영양 정보를 상세 화면에 연결했습니다. [담당 작업과 PR](https://github.com/taein0926/taein0926/blob/main/projects/zipbap-coin/README.md)
- **PinUp** — 지도 기반 맛집 리뷰의 검색바와 가게 카드를 개발하고, 목록과 리뷰 상세를 오갈 때 헤더가 바뀌도록 연결했습니다. [담당 작업과 PR](https://github.com/taein0926/taein0926/blob/main/projects/pinup/README.md)
- **GDGoC INHA 모집 웹페이지** — 모바일 너비에 맞춰 레이아웃을 조정하고, 브라우저 높이가 바뀌면 표시 영역의 높이를 다시 계산했습니다. [모바일 대응 PR](https://github.com/GDGoCINHA/23-24_Web_Promotion_Landing_Page/pull/2) · [높이 처리 PR](https://github.com/GDGoCINHA/23-24_Web_Promotion_Landing_Page/pull/4)
