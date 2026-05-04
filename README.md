# 🪖 락뱃 고상파 (ROKBATT 고상파)

> **ROKBATT UNP 2-5 상황병 전용 당직 관리 및 신속 상황보고 시스템**  
> `v3.3.0` · Lebanon EEST (UTC+3) · [🔗 바로가기](https://taedragon0112.github.io/ROKBATT_GOSANGPA/)

---

## 📋 개요

레바논 파병 유엔 평화유지군(ROKBATT UNP 2-5) 상황병이 사용하는 단일 페이지 웹 애플리케이션입니다.  
SALTR/FIR 상황보고 자동 생성, 사건 대시보드, 인수인계 체크리스트, 배차 관리, 커뮤니티 등 당직 운용에 필요한 기능을 하나의 파일에 통합했습니다.

---

## ⚙️ 주요 기능

### 📡 상황 보고 생성기
- **SALTR 자동 생성** — FIRING, NEWIMPACT, INTERCEPT, MEDEVAC, WILDFIRE 등 상황 유형별 양식 자동 완성
- **UTM 좌표 입력** → 지도 위치 즉시 확인
- **FIR 연동** — 보고서 생성과 동시에 FIR 초안 자동 작성
- **로그 저장** — 생성된 보고 기록을 날짜별 캘린더로 관리

### 🗺️ 사건 대시보드
- Leaflet 지도 위 FIRING/NEWIMPACT/INTERCEPT 마커 표시
- 종심 기준점(`36N 709504 3684345`) 중심 거리 링 표시
- 사건 추이 라인차트, 시간대 히트맵, 방향별 레이더차트
- 기간 필터 (오늘 / 7일 / 30일 / 전체)

### 📋 당직 인수인계
- 체크리스트 항목 추가/완료/삭제
- 공지사항 등록 및 실시간 Firebase 공유

### 🚗 배차 관리
- 출동 기록 생성, 수정, 캘린더 조회

### 🖼️ 락뱃 갤러리
- GitHub API 기반 이미지 업로드 및 공유
- 주간 식단표 이미지 동적 업로드 (Firebase 연동)

### 💬 커뮤니티
- 게시글 작성, 댓글, 이미지 첨부
- 비밀번호 기반 게시글 보호

### 📈 마켓 티커
- 하단 고정 바 — FX(달러/원, 유로 등), BTC/ETH, 금(XAU/USD), 미국 주요 주식 실시간 표시

---

## 🛠️ 기술 스택

| 항목 | 내용 |
|------|------|
| 구조 | 단일 파일 (`index.html`) |
| 호스팅 | GitHub Pages |
| DB | Firebase Realtime Database (compat SDK) |
| 지도 | Leaflet.js |
| 차트 | Chart.js |
| 이미지 | GitHub API |
| 마켓 데이터 | Twelve Data API, open.er-api.com, CoinGecko |
| 시간대 | Lebanon EEST (UTC+3) |

---

## 🚀 접속

```
https://taedragon0112.github.io/ROKBATT_GOSANGPA/
```

별도 설치 없이 링크만으로 접속 가능합니다.

---

## 📦 배포

```bash
git add .
git commit -m "update"
git push
```

`main` 브랜치 push 시 GitHub Pages 자동 배포됩니다.

---

## 📁 구조

```
ROKBATT_GOSANGPA/
├── index.html     # 전체 앱 (HTML + CSS + JS)
└── README.md
```

---

## 📅 버전 이력

| 버전 | 날짜 | 주요 변경 |
|------|------|-----------|
| v3.3.0 | 2026.03.27 | 서머타임 UTC+3 적용, Firebase 리스너 재작성 |
| v3.1.0 | 2026.03.26 | 사건 대시보드 추가 |
| v3.0.0 | 2026.03.24 | Firebase 연동, GitHub Pages 호스팅 |
| v2.4.x | 2026.03.24 | 배차 관리, 커뮤니티, 마켓 티커 |

---

<div align="center">
  <sub>🇺🇳 ROKBATT UNP 2-5 · Lebanon · 2026</sub>
</div>
