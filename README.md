# KPE Archive Showcase

KPE Archive 진열창 사이트입니다. 01~30편마다 서시와 이야기별 한 장면을 사진, 설명, 낭독으로 보여줍니다.

- 기준: 통합 마스터 v41 (2026-11-26), KPE_VolNN_ENKR_Overlay_FXL
- 작성: 2026-11-26

## 폴더 구성

| 위치 | 내용 |
| --- | --- |
| index.html | 진열창 페이지 (틀 하나로 30편 모두 보여줌) |
| data/volumes.json | 진열창 권 목록 |
| data/KPE_VolNN_Showcase.json | 권별 장면의 글·사진·음원 정보 (MCP 서버도 이 파일을 읽음) |
| data/showcase_data.js | 위 JSON을 한데 모은 파일 (컴퓨터에서 바로 열 때 쓰임) |
| images/ | 장면 사진 |
| audio/ | 서시 미리듣기와 사진 설명 낭독 |

주소 끝에 `#vol-01`처럼 붙이면 그 권이 바로 열립니다. 아무것도 없으면 30편 목록이 나옵니다.

## GitHub에 올리는 순서

1. GitHub에서 새 공개 저장소를 만듭니다. 이름 예: `kpe-showcase`
2. 이 폴더 안의 파일과 폴더를 그대로 올립니다 (index.html이 맨 위에 있어야 합니다).
3. 저장소 **Settings → Pages**에서 Branch를 `main`, 폴더를 `/ (root)`로 정하고 저장합니다.
4. 몇 분 뒤 `https://<계정>.github.io/kpe-showcase/` 주소로 열립니다.

## 고칠 때

- 문구나 감정 태그를 고치면 `data/KPE_VolNN_Showcase.json`과 `data/showcase_data.js`를 함께 바꿉니다. Claude에게 통합 마스터 최신본을 주시면 둘 다 다시 만들어 드립니다.
- 구매 링크는 각 JSON의 `buy_link`입니다. 권별 아마존 킨들 도서 주소(https://www.amazon.com/dp/ASIN)입니다.

## 원칙

- 공개 저장소에는 진열창에 여는 내용만 둡니다.
- 포토 디스크립션 전문, 본문 원문, 시구, 고해상 원본은 올리지 않습니다.
