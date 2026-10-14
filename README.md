# 상가업소 검색 지도

## 실행
`index.html`을 Chrome 또는 Edge에서 열고 CSV를 선택합니다. CSV 업로드만으로는 마커가 표시되지 않습니다. 상호명 검색 후 일치한 매장만 지도에 표시됩니다.

## 필수 컬럼
`상호명`, `지점명`, `도로명`, `경도`, `위도`
원본 파일에 `도로명주소`만 있다면 해당 열 이름을 `도로명`으로 바꾸거나 HTML의 필수 컬럼 코드를 수정하세요.

## 기능
- CSV 업로드 및 필수 컬럼 검증
- 상호명 부분 일치 검색
- 검색 결과만 지도 마커로 표시
- 마커 클릭 시 상호명, 지점명, 도로명 표시
- CSV(UTF-8 BOM) / GeoJSON 다운로드
- 좌표가 유효하지 않은 행은 지도와 GeoJSON에서 제외
- 파일은 브라우저에서 처리되며 애플리케이션 서버로 전송하지 않음

## GitHub Pages
1. GitHub 저장소 최상위에 `index.html`과 `README.md`를 업로드합니다.
2. Settings → Pages → Build and deployment에서 `Deploy from a branch`를 선택합니다.
3. Branch `main`, folder `/(root)`를 선택하고 Save를 누릅니다.
4. 생성된 HTTPS 주소로 접속합니다.

Leaflet, PapaParse 및 OpenStreetMap 타일을 온라인에서 불러오므로 인터넷 연결이 필요합니다.
