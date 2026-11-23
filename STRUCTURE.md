# STRUCTURE · aubeeair-sample (v0.2 · 흰 바탕 + 로고 하늘색 패널(물빛 무늬) · AUB 워드마크 · 눈 클로즈업 · 모서리 2px · 배포 예정 aubeeair-sample.lgt3232.workers.dev)

```
aubeeair-sample/
├─ index.html                 단일 파일 (CSS · JS 인라인)
├─ wrangler.toml              name = aubeeair-sample
├─ .assetsignore              img/ · _old/ · 문서 · index_*.html · _deploy 배포 제외
├─ ab-jost.woff2              영문 워드마크 · 라벨 · 섹션 제목 (Jost 300–500, 영문 · 숫자만)
├─ ab-pretendard.woff2        본문 · 한글 (Pretendard 300–700, 페이지 글자 전부)
├─ ab-hero.webp · ab-hero-m.webp  히어로 눈 클로즈업 (960×1200 · 1080×720)
├─ ab-caustic.webp           히어로 패널 물빛 무늬 타일 (512×512 투명 · 빌더 생성)
├─ ab-about.webp              About 사진 (800×1000)
├─ ab-w1 ~ ab-w8.webp         Works 시술 사진 8장 (720×900)
├─ favicon.svg · favicon.png · og-ab.jpg   하늘색 바탕 + AUB (SVG는 Jost 글자를 패스로)
├─ img/                       다올 제공 원본 + _원문.md (배포 제외 · 레포에 올리지 말 것)
└─ CHANGELOG.md / STRUCTURE.md  (로컬 정본 · 업로드 안 함, R-38)
```

## 섹션 순서
헤더 `.top`(sticky · 로고 AUB 오브에르 · PC 메뉴 + 「카카오 채널 예약」 / 900 미만 `.snav` 5칸)
→ 히어로(900 이상: 하늘 패널 | 사진 / 미만: 사진 38svh → 패널) → `#about` → `#works`(옅은 하늘) → `#price` → `#booking`(옅은 하늘 · 영업시간 표) → `#visit`(구글 지도) → 푸터(검정) + 모바일 `.quick`.

## 버튼 · 링크
- 카카오 채널 `http://pf.kakao.com/_Jugyxj`(메인): 헤더(PC) · 히어로 · 예약 · 푸터 · 하단 바
- 전화 `tel:01084244792`: 히어로 · 오시는 길 · 푸터 · 하단 바 / 0507 `tel:050713424792`: 오시는 길 "전화번호" 줄만
- 네이버 플레이스 `m.place.naver.com/place/1795726923/home`: 예약(「네이버 예약」) · 푸터 · JSON-LD / 네이버 지도 `map.naver.com/p/entry/place/1795726923`: 오시는 길
- 인스타 `instagram.com/aubeeair/`: Works 안내 · 예약 · 푸터 · 하단 바
- 구글 지도 embed 검색어 「충남 천안시 서북구 쌍용17길 25」 (배포 후 핀 확인 필요 · R-35)

## 모션 (강제 재생)
- 히어로 `.intro` 등장 · 패널 물빛 무늬 두 겹 흐름(setInterval 50ms → `--w1` · `--w2` background-position) · `.reveal`(setInterval · `.js` 게이팅) · 앵커 rAF 스크롤(R-25). reduced-motion 분기 없음.

## 폰트 재생성
문구 바꾸면 빠진 글자 검사(LESSONS §26). Pretendard 원본 `fonts/Pretendard-1.3.9/public/variable/PretendardVariable.ttf`(300–700) · Jost `fonts/fonts-main/ofl/jost/Jost[wght].ttf`(300–500, 영문만).
