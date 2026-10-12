# 냥냥아일랜드 웹사이트 (Meow Meow Island)

정적 사이트 — 빌드 없음. `index.html` 하나가 한국어·English·日本語를 모두 그린다
(브라우저 언어로 자동 선택, 상단 버튼으로 전환, `?lang=en` 링크 가능).
`index-en.html` / `index-ja.html`은 기존 사이트와 주소를 맞추려는 리다이렉트다.

## 다운로드 링크 (유튜브·인스타 프로필용)
`https://nini-universe.github.io/meow-island-website/download/`
- 아이폰·아이패드 → 0.5초 뒤 App Store로 자동 이동
- 안드로이드 → Play 출시 전엔 "곧 출시" 안내 + 소개 페이지 버튼.
  **출시 후 `download/index.html`의 `PLAY_URL` 한 줄만 채우면** 자동 이동한다
- PC → 자동 이동 없이 App Store·소개 페이지 버튼
- 인스타·유튜브 앱 안 브라우저가 자동 이동을 막아도 버튼이 남아 있어 직접 누를 수 있다
- 메인 소개 페이지(`/meow-island-website/`)는 자동 이동하지 않는다 — 폰에서도 소개를 볼 수 있게

## 배포 (GitHub Pages)
1. GitHub `nini-universe`에 저장소를 만들어 이 폴더를 올린다 (예: `meow-island-website`)
2. Settings › Pages › Branch `main` / root
3. App Store Connect › 앱 정보 › **마케팅 URL**에 사이트 주소를 넣는다
   — AdMob은 개발자 웹사이트 **루트**의 `app-ads.txt`를 읽는다. 그래서 사이트 주소는
   `https://<도메인>/` 형태(하위 경로 X)여야 한다. `<org>.github.io/<repo>/`처럼 하위 경로면
   맞춤 도메인을 붙이거나 `<org>.github.io` 저장소에 app-ads.txt를 둔다.

## 그림 출처
게임 저장소(`cat_island`)의 에셋을 그대로 줄여 썼다 — 아이콘, 헤더 렌더(`integration_test/header_art_test.dart`),
스토어 스크린샷, 휴양지 고양이 프레임(게임과 같은 간격으로 돌린다).
