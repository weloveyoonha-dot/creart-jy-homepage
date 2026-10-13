# 크리아트 일산주엽원 GitHub Pages 홈페이지

## 1. 먼저 GitHub 기본 주소로 시험 배포
1. GitHub에서 공개 저장소 `creart-homepage`를 만듭니다.
2. 이 압축파일 안의 **파일과 assets 폴더**를 저장소 최상위에 업로드합니다. (압축파일 자체를 올리지 마세요.)
3. Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.
4. `https://사용자명.github.io/creart-homepage/`에서 확인합니다. 배포에 몇 분 걸릴 수 있습니다.
5. 이 단계에서는 가비아 DNS를 수정하지 않습니다.

## 2. 공개 전 필수 확인
- 전화번호 `010-6795-6884`와 주소 `경기도 고양시 일산서구 강선로 33`이 현재 실제 정보와 일치하는지 확인하세요.
- 정식 등록명, 대상 연령, 수업 내용 및 체험수업 운영 여부를 확인하세요.
- 상단의 그림과 갤러리는 **실제 수업 사진이 아닌 CSS 디자인 그래픽**입니다.
- 실제 수업 사진을 넣으려면 `assets/`에 웹용 사진을 업로드하고 HTML의 해당 구역을 이미지로 바꾸세요. 보호자 동의를 확인하세요.
- 현재 네이버 블로그/플레이스 링크는 제공받은 공식 주소를 사용합니다.
- 외부 폰트(Google Fonts)를 사용합니다. 인터넷 연결이 없으면 기본 폰트로 표시됩니다.

## 3. 도메인 이전은 홈페이지 완성 후
1. GitHub Pages의 Custom domain에 `www.creart-jy.com` 등록.
2. 가비아 포워딩 설정을 해제하고 포워딩 서비스가 만든 A 레코드를 정리.
3. 루트(@)에 GitHub Pages A 레코드 4개를 등록: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
4. `www` CNAME을 `사용자명.github.io.`로 변경. 기존 Google Sites CNAME 및 동일 www 호스트의 A 레코드가 함께 남지 않도록 합니다.
5. DNS 반영 후 GitHub Pages에서 Enforce HTTPS를 켭니다. 루트와 www 모두 테스트하세요.
6. DNS 값과 정책은 실제 전환 시점에 GitHub 공식 문서에서 다시 확인하세요: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## 4. SEO
- `index.html`의 title, description, canonical, JSON-LD 확인.
- `robots.txt`와 `sitemap.xml`은 **최종 도메인용**입니다. 시험 주소에서 색인을 서두르지 마세요.
- Google Search Console 및 네이버 서치어드바이저에 최종 도메인을 등록하고 사이트맵을 제출하세요.
- AI 검색 노출이나 추천을 보장하는 설정은 아닙니다.

## 파일 구조
`index.html`, `style.css`, `script.js`, `robots.txt`, `sitemap.xml`, `.nojekyll`, `assets/favicon.svg`
