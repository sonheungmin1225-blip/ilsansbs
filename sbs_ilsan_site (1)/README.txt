SBS아카데미게임학원 일산점 홈페이지 (정적 사이트)

[Vercel 배포]
1) vercel.com → Add New → Project → 이 폴더(압축 해제한 폴더)를 GitHub 저장소에 올린 뒤 Import
   (또는 터미널에서 이 폴더로 이동해 `npx vercel --prod`)
2) Framework Preset: Other / Build Command: 비움 / Output Directory: 비움(루트)
3) Deploy

[주소 구조]
/                      홈
/blog/                 학원 이야기 목록
/blog/<글주소>/         학원 이야기 글 (8편)
/ilsan-game/ 등         지역·과목별 안내 (8개: 일산게임·일산웹툰·일산미술·일산게임프로그래밍·운정게임·파주웹툰·화정게임·김포게임)
/courses/ /support/ /campus/ /news/ /consult/ /about/

[파일]
assets/site.css  스타일
assets/app.js    내용·동작 (지점 정보 BRANCH, 예약 BOOK, 글 posts)
assets/*.webp    이미지
각 폴더의 index.html은 검색엔진용으로 미리 그려 둔 페이지입니다.
글을 추가·수정하면 검색엔진용 index.html도 다시 생성해야 합니다.
