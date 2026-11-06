# 특별관 장르 적합도 대시보드

김지민 · CJ 4DPLEX 사전과제

한국 KOBIS 상영타입별 데이터로 특별관(4D·ScreenX)에 잘 맞는 장르를 찾고, 해외 박스오피스 트렌드에 대입한 분석 대시보드입니다.

## 폴더 구성
- `index.html` : 대시보드 페이지
- `assets/dash.js` : 데이터를 읽고 차트를 그리는 작은 런타임 (d3 v7 사용)
- `data/*.csv` : 분석 결과 데이터
  - `kr_format.csv` 포맷별 일반관 대비 배수 요약 (KOBIS)
  - `kr_buckets.csv` 장르 묶음별 4D·ScreenX 배수 (KOBIS)
  - `kr_films.csv` 작품별 배수 108편 (KOBIS)
  - `kr_tests.csv` 통계 검정 결과
  - `global_share.csv` 전 세계 Top50 장르 비중 (Box Office Mojo)
  - `market_year.csv` 해외 12개 시장 연도별 장르 비중
  - `horror_kr.csv` 전 세계 흥행 상위 공포의 한국 상영 현황 (KOBIS)

## GitHub Pages로 올리기
1. 이 폴더의 파일을 저장소 맨 위(루트)에 올립니다.
2. 저장소 Settings → Pages → Branch를 `main` / `/ (root)`로 저장합니다.
3. 잠시 뒤 `https://<아이디>.github.io/<저장소이름>/` 에서 열립니다.

로컬에서 확인할 때는 파일을 직접 열지 말고 간단한 서버로 여세요 (CSV를 읽기 때문):
`python -m http.server` 실행 후 http://localhost:8000
