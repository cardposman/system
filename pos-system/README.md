# 밴포스시스템 GitHub Pages 랜딩페이지

이 패키지는 `cardposman.github.io` 공용 도메인의 하위 경로인 `/pos-system/`에 업로드하도록 제작되었습니다.

## 포함 페이지

총 10개 페이지가 포함되어 있습니다.

- 홈: `/pos-system/`
- 카드단말기: `/pos-system/card-terminal/`
- 포스기: `/pos-system/pos/`
- 키오스크: `/pos-system/kiosk/`
- 테이블오더: `/pos-system/table-order/`
- 음식점: `/pos-system/restaurant/`
- 카페: `/pos-system/cafe/`
- 주점/호프: `/pos-system/pub/`
- 신규 창업 매장: `/pos-system/startup/`
- 결제장비 비교 가이드: `/pos-system/guide/`

## 업로드 방법

1. ZIP 파일을 압축 해제합니다.
2. `pos-system` 폴더 전체를 기존 GitHub Pages 저장소 루트에 업로드합니다.
3. 업로드 후 아래 주소로 접속합니다.

`https://cardposman.github.io/pos-system/`

## 전화번호와 네이버폼 URL 교체

아래 파일을 열어 임시값을 실제 값으로 교체하세요.

`pos-system/assets/js/main.js`

```js
const PHONE_NUMBER = '88888888';
const NAVER_FORM_URL = 'nnnnnnnn';
```

전화 연결과 네이버폼 이동은 모두 `button onclick` 방식으로 처리되어 있습니다. 내부 페이지 이동 링크만 검색엔진 수집을 위해 `<a href>` 방식으로 유지했습니다.

## robots.txt 안내

패키지 안에 `pos-system/robots.txt`가 포함되어 있습니다. 다만 검색엔진은 보통 도메인 루트의 robots.txt를 우선 확인합니다.

기존 루트 robots.txt가 있다면 덮어쓰지 말고 아래 줄만 추가하세요.

`Sitemap: https://cardposman.github.io/pos-system/sitemap.xml`

## 네이버 서치어드바이저 등록 순서

1. `https://cardposman.github.io/pos-system/` 접속 확인
2. 네이버 서치어드바이저에서 사이트 등록 또는 기존 사이트 관리 접속
3. 사이트맵 제출: `https://cardposman.github.io/pos-system/sitemap.xml`
4. 주요 페이지 수집 요청

## 제작 메모

- 사은품 내용은 본문에서 제외했습니다.
- 선불형/후불형 표현은 키오스크와 테이블오더 페이지에서만 사용했습니다.
- 공식 근거가 필요한 수치, 후기, 인증, 1위 표현은 본문 텍스트에서 제외했습니다.
- 홍보력 강화를 위해 CTA와 장비 도입 장점 문구를 이전 버전보다 적극적으로 수정했습니다.
