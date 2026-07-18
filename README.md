# 나의 서재 모바일 ISBN 스캐너

스마트폰 후면 카메라로 ISBN(EAN-13) 바코드를 스캔하고 책 정보를 조회해 개인 서재에 저장하는 PWA입니다.

## 사용 조건
- 스마트폰 Chrome 또는 Safari 최신 버전
- 카메라 기능은 HTTPS 주소에서만 작동
- 책 정보 조회와 사진 스캔 보조 모듈에는 인터넷 연결 필요

## 권장 배포
이 폴더 전체를 GitHub Pages, Netlify, Vercel 등 HTTPS 정적 호스팅에 올린 뒤 스마트폰에서 해당 주소를 엽니다.

## 기능
- 후면 카메라 우선 실행
- 카메라 직접 선택
- ISBN EAN-13 실시간 인식
- 플래시 지원 기기에서 플래시 켜기/끄기
- 사진 촬영/선택 후 바코드 인식
- Open Library 및 Google Books 책 정보 조회
- 개인 서재와 북리뷰를 기기 브라우저에 저장
- 홈 화면 설치(PWA)


## iPhone 바코드 수정판

이 버전은 iPhone Safari에서 지원되지 않을 수 있는 `BarcodeDetector` 대신
`html5-qrcode`를 실시간 스캐너로 사용합니다.

GitHub에 기존 `index.html`과 `sw.js`를 이 버전으로 교체한 뒤,
Safari에서 페이지를 새로 열거나 홈 화면 아이콘을 삭제 후 다시 추가하세요.
