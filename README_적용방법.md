# 포트폴리오 웹사이트 — v3.1 (엄마의 약봉투 15초 영상)

**작성일:** 2026-04-18 (v3.1)
**변경 요약:** v3(전체 리뉴얼)에 **"엄마의 약봉투" 15초 숏폼 영상**이 실제로 제작되어 포트폴리오 안에서 재생됩니다. 샘플 카드에 "15초 영상 보기" 버튼이 생기고, 클릭하면 Instagram Reels 포맷(9:16)으로 모달에서 재생됩니다.

---

## 🎬 엄마의 약봉투 — 15초 스토리보드

| 시간 | 씬 | 카피 | 비주얼 |
|---|---|---|---|
| 0–1.5s | Hook | "엄마가 꺼낸 약봉투 세 개." | 어두운 테이블 + 스포트라이트 + 약봉투 3개 |
| 1.5–3s | Problem | "어라, 이거 언제 먹는 거더라?" | 라벨 클로즈업 (고혈압·당뇨·콜레스테롤) |
| 3–5s | Daughter | "딸이, 사진을 찍는다." | 폰 하강 + 카메라 뷰파인더 UI |
| 5–6s | Shutter | (플래시) + "+Healthier · 약봉투 인식 중…" | 셔터 플래시 → 퍼플 브랜드 전환 |
| 6–10s | Solution | "약 3개를 찾았어요 · 복용 시간을 정리해 드렸어요." | 3 pill cards: 암로디핀/메트포르민/로수바스타틴 + 각 복용 시간 |
| 10–12s | Payoff | "엄마, 이 약은 이때 드시면 돼." | 타이포그래피 + 워밍업 크림톤 |
| 12–13s | Emotion | "그리고, 엄마가 웃었다." | 따뜻한 그라디언트 |
| 13–15s | Brand | "검색 대신, 물어보세요." / "건강 걱정 안해도 되는 시대" | Healthier 로고 + App Store/Google Play CTA |

**감정 곡선:** 거리감 → 당혹 → 개입 → 안도 → 연결 → 웃음 → 확신 (7단)

**헬시어 통합 방식:**
- 6초 이전에는 브랜드 등장 NO — 감정 공감 먼저
- 6–10초: 실제 앱 UX 플로우 재현 (카메라 → AI 인식 → 복용 시간표)
- 엔딩은 제품 판매 아니라 **"엄마가 웃는다"** — 메디올로지 미션 그대로

**스펙:** 1080×1920 (9:16) · 24fps · 360 frames · 15초 · H.264 · 607KB

---

## 📦 이 폴더의 v3.1 파일들

```
99_웹사이트_업로드/
├── index.html                  ← +160줄 (영상 버튼 CSS/HTML/JS + 모달)
├── mom-medicine-pouch.mp4      ← 신규 · 607KB · 15초 시네마틱
├── strategy.html               ← 기존 (v3)
├── strategy.md                 ← 기존 (v3)
├── mediology-ad.mp4            ← 기존 (v2 히어로 30초)
└── assets/samples/             ← 기존 (v2 카드뉴스 24장)
```

---

## 🚀 배포 (Mac 터미널 — 한 줄)

```bash
cd ~/Documents/github/reverse-aging-portfolio && \
cp "/Users/kooking1/Documents/Claude/Projects/메디올로지 의료ai 스타트업 최고마케터 (CMO)/99_웹사이트_업로드/index.html" ./index.html && \
cp "/Users/kooking1/Documents/Claude/Projects/메디올로지 의료ai 스타트업 최고마케터 (CMO)/99_웹사이트_업로드/mom-medicine-pouch.mp4" ./mom-medicine-pouch.mp4 && \
git add index.html mom-medicine-pouch.mp4 && \
git -c user.email="godscience2024@gmail.com" -c user.name="구건우" commit -m "v3.1 — 엄마의 약봉투 15초 숏폼 영상 + 카드 모달 재생" && \
git push origin main
```

**파인더 방식:**
1. `99_웹사이트_업로드` 폴더 열기
2. `index.html`과 `mom-medicine-pouch.mp4` 2개를 `~/Documents/github/reverse-aging-portfolio/`로 드래그 (덮어쓰기)
3. 터미널에서 `git add -A && git commit -m "v3.1" && git push`

---

## ✅ 배포 후 확인 (https://reverse-aging-portfolio.vercel.app/)

1. **Samples 섹션으로 스크롤** → 3번째 블록 "엄마의 약봉투" 타일
2. 타일 안에 **"▶ 15초 영상 보기"** 그린 버튼 + "실제 제작 완료 · 0.6 MB" 서브 텍스트
3. 버튼 클릭 → 중앙에 9:16 모달 등장, 영상 자동 재생
4. 오른쪽 상단 ✕ 또는 ESC로 닫기
5. 모바일: 세로 꽉 차는 모달, 컨트롤 바 하단

**직접 재생 URL:** https://reverse-aging-portfolio.vercel.app/mom-medicine-pouch.mp4

---

## 🎯 대표님께 설명하실 때

> "샘플 카드에 있던 '엄마의 약봉투' 컨셉, 그대로 영상으로 만들어 붙였습니다.
>
> **핵심 3가지:**
>
> 1. **감정 곡선을 먼저 설계** — 거리감 → 당혹 → 안도 → 웃음 → 확신. 제품이 아니라 이야기를 먼저.
>
> 2. **헬시어는 6초 이후 등장** — 앞 5초는 완전히 엄마-딸 관계의 이야기. 광고가 아니라 '아, 내 이야기다'로 느끼도록.
>
> 3. **엔딩은 다운로드가 아니라 '엄마가 웃었다'** — 메디올로지 미션 '건강 걱정 안해도 되는 시대'를 영상 마지막 2초에 그대로 얹었습니다.
>
> **시리즈로 확장 가능**: #오늘의약봉투 1편 '엄마 편', 2편 '시부모님 편', 3편 '반려동물 약 편'… 포맷은 고정, 이야기만 교체. 콘텐츠 팀이 주 2회 발행하는 구조로 쉽게 갈 수 있습니다."

---

*구건우 | 2026-04-18 v3.1 (엄마의 약봉투 영상)*
