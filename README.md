# PRISM 광고 대시보드

## 파일 구조
```
/
├── index.html          → 대행사용 (전체 탭)
├── client/index.html   → 광고주용 (쇼핑랭킹 제외)
├── admin/index.html    → 관리자 (데이터 업로드)
├── data/
│   ├── ad_data.json        ← 4월/5월 광고성과 (관리자 업로드)
│   ├── naver_best_rankings.json  ← 쇼핑베스트 (자동 업데이트)
│   ├── trend_data.json     ← 검색트렌드 (자동 업데이트)
│   ├── shopping_insight.json ← 쇼핑인사이트 (자동 업데이트)
│   ├── competitor_events.json ← 경쟁사 모니터링 (자동 업데이트)
│   └── meta_ads.json       ← 메타 광고 (자동 업데이트)
└── scrapers/               ← GitHub Actions 스크래퍼
```

## 배포
- Cloudflare Pages 연결: `prism.22brix.co.kr`
- 광고주 URL: `prism.22brix.co.kr/client`
- 관리자 URL: `prism.22brix.co.kr/admin`

## 자동 업데이트
매일 자정 GitHub Actions 실행 → data/ 폴더 갱신 → Cloudflare 자동 배포

## 관리자 비밀번호
prism2026
