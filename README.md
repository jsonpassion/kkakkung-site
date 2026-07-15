# kkakkung-site

[까꿍](https://github.com/jsonpassion/Kkakkung)(Kkakkung) — 아기가 웃는 순간을 자동으로 포착하는 iOS 카메라 —
의 소개 웹사이트와 법적 문서 저장소.

배포: GitHub Pages (`main` 브랜치의 `/docs`)
→ https://jsonpassion.github.io/kkakkung-site/

## 구조

```
docs/
├── index.html    # 랜딩 페이지 (쓰는 법, Lottie 모션, 기능, 데모, 가격, FAQ)
├── privacy.html  # 개인정보 처리방침 (한국어/영어)
├── terms.html    # 이용약관 (한국어/영어)
├── styles.css    # 웜 daylight 테마 공용 스타일 (살구/크림)
└── lottie/
    ├── smile-capture.json   # 웃음 게이지 → 자동 촬영
    ├── peekaboo.json        # 까꿍 놀이 → 눈 맞춤
    ├── on-device.json       # 아기 사진은 폰 안에서만
    └── lottie_light.min.js  # self-hosted bodymovin 플레이어 (CDN 미의존)
```

Lottie 3종은 `bodymovin 5.7.4` 셰이프로 손수 제작(툴 없이 코드 생성).
순수 정적 HTML/CSS/JS — 빌드 단계 없음.

## 운영 메모

- App Store 출시 후 `index.html`의 스토어 배지 `href`(`TODO` 주석 위치)를 실제 링크로 교체할 것.
- 정책 문서를 수정하면 문서 상단의 "최종 수정일/시행일"도 함께 갱신할 것.
- 사업자 표기: ForgeLab · 대표 Jason Lee · forgelab.aitech@gmail.com

© 2026 ForgeLab
