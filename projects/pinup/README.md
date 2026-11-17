# PinUp — 프론트엔드 담당 작업

지도에서 가게와 리뷰를 찾아보는 팀 프로젝트입니다.
저는 React·TypeScript로 검색바, 가게 카드·이미지 슬라이더, 목록과 리뷰 상세 화면의 전환을 개발했습니다.

- [팀 원본 저장소](https://github.com/TEAM-PIN-UP/FE-PIN-UP) · 기준 브랜치: `dev`
- 이 문서는 담당한 프론트엔드 작업을 정리한 소개 페이지입니다. 팀 전체 구현은 원본 저장소에서 확인할 수 있습니다.

## 담당 작업과 근거

| 작업 | 구현 내용 | 본인 PR |
| --- | --- | --- |
| 검색바와 가게 카드 | 입력·포커스·초기화에 따른 아이콘과 동작, 가게 정보 카드, 공통 Swiper를 활용한 이미지 슬라이더 | [#20](https://github.com/TEAM-PIN-UP/FE-PIN-UP/pull/20) |
| 화면 전환 | 가게 목록에서 리뷰 상세 화면으로 전환, 상태에 따른 헤더 변경과 뒤로가기 연결 | [#37](https://github.com/TEAM-PIN-UP/FE-PIN-UP/pull/37) |
| 스타일 보완 | 기존 글꼴 정의 B3 적용, 개별 고정 글꼴 크기 제거 | [#58](https://github.com/TEAM-PIN-UP/FE-PIN-UP/pull/58) |

TypeScript를 처음 사용하는 단계에서 PR에 타입 검토를 요청했습니다. 검색바 상태 타입을 명시해 달라는 리뷰를 반영하고, 이후 화면 동작과 스타일 변경도 PR 검토를 거쳐 팀 브랜치에 통합했습니다.

## 코드에서 볼 부분

- [검색바](https://github.com/TEAM-PIN-UP/FE-PIN-UP/blob/dev/src/components/SearchBar.tsx): 입력 상태와 포커스·초기화 처리
- [지도 화면](https://github.com/TEAM-PIN-UP/FE-PIN-UP/blob/dev/src/pages/Map/index.tsx): 목록과 리뷰 화면의 전환 흐름
- [공통 Swiper](https://github.com/TEAM-PIN-UP/FE-PIN-UP/blob/dev/src/components/BasicSwiper.tsx): 이미지 슬라이더에 사용하는 래퍼

## 기술과 범위

본인 담당 화면에는 TypeScript, React, styled-components, Swiper를 사용했습니다.
팀 저장소에는 지도와 API 연동 등 다른 팀원의 작업도 포함되어 있습니다. 위 PR의 화면 작업을 서비스 전체나 검색 API 전체의 단독 구현으로 설명하지 않습니다.
초기 카드·이미지 구현에는 예시 데이터가 포함되어 있으므로, 화면 구현과 실제 데이터 연동은 구분해서 볼 수 있습니다.

Storybook을 구축한 프로젝트는 아닙니다. 기존 글꼴·간격 기준을 적용하고 컴포넌트의 상태와 화면 전환을 다룬 경험을 보여 줍니다.

## 원본 실행 참고

원본 저장소를 받은 뒤 `package.json`의 스크립트로 실행합니다.

```bash
yarn install
yarn dev
```

`yarn build`는 TypeScript 검사와 Vite 빌드를, `yarn lint`는 ESLint 검사를 실행합니다.
지도·서버 기능에는 원본 저장소의 환경 설정과 외부 서비스가 필요합니다. 이 문서 변경 과정에서는 애플리케이션을 실행하거나 배포 상태를 확인하지 않았습니다.
