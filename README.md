#이지램스(ezREMS) 웹페이지 디자인 가이드 v0.1

파일명 | 용도
ezrems-design-system.zip     전체 프로젝트 폴더 (분리된 파일 구조)
ezrems-preview.html           단일 실행 가능한 미리보기 HTML


📁 ZIP 압축 파일 구조

ezrems-design-system/
├── index.html            (14KB) ← 임대계약관리 표준 템플릿
├── README.md                    ← 사용 가이드
├── css/
│   ├── variables.css     (1.3KB) ← CSS 변수 (색상/폰트/간격)
│   ├── base.css          (0.9KB) ← 리셋 + 기본 스타일
│   ├── layout.css        (4.9KB) ← GNB, 탭바, 스플릿 레이아웃
│   └── components.css    (6.0KB) ← 버튼, 배지, 폼, 테이블
└── js/
    ├── common.js          (6.7KB) ← 공통 유틸리티 (날짜, 숫자, DOM, Toast, Ajax)
    └── page.js            (7.0KB) ← 페이지 비즈니스 로직 (샘플 데이터 포함)


✅ 동작 확인 (미리보기 화면에서 테스트 완료)

GNB 메뉴 + 탭바 — 원본과 동일한 구조
검색 필터 + 조회 버튼 — 클릭 시 로딩 스피너 → 결과 표시 + 성공 Toast
테이블 행 선택 — 클릭 시 파란 배경 하이라이트 + 왼쪽 파란 border
날짜 배지 — 만료/임박/미래 날짜별 색상 자동 적용
태그 배지 (쥬라기, 101 등) — 회색 배경 태그
엑셀 버튼 — CSV 파일 자동 다운로드
삭제 버튼 — confirm 확인창 → 삭제 Toast
아래로 이동 버튼 — 스크롤 이동



🚀 새 페이지 만들기 방법

index.html 복사 → 새 페이지명으로 저장
js/page.js 복사 → 페이지별 데이터/로직으로 교체
css/variables.css의 CSS 변수만 수정하면 전체 테마 변경 가능



ezrems-preview.html 파일은 
외부 의존성 없이 바로 브라우저에서 열면 동작합니다!
