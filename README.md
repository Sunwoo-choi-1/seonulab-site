# AI로 다했서누 — 공식 웹페이지

서누랩(seonulab) 개인 브랜드 웹페이지. 프레임워크 없는 순수 정적 사이트라 빌드 과정이 필요 없습니다.

## 구조

- `index.html` — 페이지 전체 (HTML + CSS + 이메일 복사 스크립트)
- `assets/banner-lockup.png` — 히어로 배너 (유튜브 배너 크롭)
- `assets/profile.jpg` — 프로필 사진 (파비콘 겸용)

## Vercel 배포

1. [vercel.com](https://vercel.com)에서 **Continue with GitHub**으로 로그인
2. **Add New → Project** → 이 저장소(`seonulab-site`) **Import**
3. 설정은 그대로 두고 **Deploy** 클릭 (Framework Preset: Other, 빌드 명령 없음)
4. 완료되면 `https://<프로젝트명>.vercel.app` 주소가 생깁니다

이후에는 이 저장소의 `main` 브랜치에 푸시할 때마다 자동으로 재배포됩니다.

## 자체 도메인 연결

1. Vercel 프로젝트 → **Settings → Domains**
2. 도메인 입력 (예: `seonulab.com`) → 구매했다면 안내에 따라 DNS 레코드(A/CNAME) 추가
   - Vercel에서 바로 구매하면 DNS 설정이 자동으로 됩니다
3. 연결 후 `index.html` 상단의 `og:url`, `og:image`, `twitter:image` 주소를 새 도메인으로 교체
