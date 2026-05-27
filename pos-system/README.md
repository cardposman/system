# 밴포스시스템 GitHub Pages 랜딩페이지

이 패키지는 `cardposman.github.io`의 기존 사이트를 덮어쓰지 않도록 `pos-system/` 하위폴더 구조로 제작되었습니다.

## 포함 페이지

1. 홈: `/pos-system/`
2. 카드단말기: `/pos-system/card-terminal/`
3. 포스기: `/pos-system/pos/`
4. 키오스크: `/pos-system/kiosk/`
5. 테이블오더: `/pos-system/table-order/`
6. 음식점: `/pos-system/restaurant/`
7. 카페: `/pos-system/cafe/`
8. 주점/호프: `/pos-system/pub/`
9. 신규 창업 매장: `/pos-system/startup/`
10. 결제장비 비교 가이드: `/pos-system/guide/`

## 주요 파일

- `index.html`
- `sitemap.xml`
- `robots.txt`
- `README.md`
- `assets/css/style.css`
- `assets/js/main.js`
- `assets/images/`

## 업로드 방법

ZIP 압축을 풀면 `pos-system/` 폴더가 나옵니다. 이 폴더를 GitHub Pages 저장소 루트에 그대로 업로드하세요.

예상 주소:

```text
https://cardposman.github.io/pos-system/
```

## 임시값 교체 위치

현재 전화번호와 네이버폼 URL은 임시값입니다.

파일:

```text
pos-system/assets/js/main.js
```

교체 대상:

```javascript
const PHONE_NUMBER = '88888888';
const NAVER_FORM_URL = 'nnnnnnnn';
```

`NAVER_FORM_URL`에는 `https://`로 시작하는 실제 네이버폼 주소를 넣는 것을 권장합니다.

## 외부 이동 방식

전화 상담과 네이버폼 이동은 `<a href>`가 아니라 `button onclick` 방식으로 구성되어 있습니다.

## robots.txt 주의사항

검색엔진이 표준으로 확인하는 robots.txt는 일반적으로 도메인 루트입니다.

```text
https://cardposman.github.io/robots.txt
```

기존 루트 robots.txt가 있다면 덮어쓰지 말고 아래 줄만 추가하세요.

```text
Sitemap: https://cardposman.github.io/pos-system/sitemap.xml
```

## 네이버 서치어드바이저 등록 순서

1. GitHub Pages에 `pos-system/` 폴더 업로드
2. 브라우저에서 `https://cardposman.github.io/pos-system/` 접속 확인
3. 네이버 서치어드바이저에서 사이트 소유 확인
4. 사이트맵 제출: `https://cardposman.github.io/pos-system/sitemap.xml`
5. 웹 페이지 수집 요청에 주요 URL 제출

## 제작 기준

- 증정 이벤트 영역은 본문과 삽입 이미지에서 사용하지 않았습니다.
- 선불형/후불형 표현은 키오스크와 테이블오더 페이지에만 사용했습니다.
- 제공된 상품홍보 이미지와 입력 정보를 기준으로 보수적인 문구를 사용했습니다.
- 공식 근거가 없는 수치, 후기, 인증, 1위 표현은 본문 텍스트에 사용하지 않았습니다.
