# CLASSLOG Web

CLASSLOG(클라쓰로그) — **AI Music Teacher Agent**를 향한 음악교육 플랫폼의 소개·콘텐츠 웹사이트입니다.

## 페이지 구성

| 파일 | 설명 |
|------|------|
| `index-classlog.html` | 회사 소개(비전·문제·솔루션·로드맵·비즈니스모델·경쟁우위·데이터전략·철학) + 첫 화면 검색바 |
| `free-sheets.html` | 무료 악보 목록 (곡별 '방'으로 연결) |
| `paid-sheets.html` | 반주 악보 · 반주 음원(MR) 판매 목록 |
| `sheet-room.html` | 곡별 상세 '방' (PDF·이미지·영상·좋아요·댓글·구매연결) |
| `mission.html` | 마일리지 미션 — 연주 업로드 → AI 진단(주법 교정 전·후 데이터 수집) |

## 배포 (Vercel)

정적 사이트입니다. 별도 빌드가 없습니다.
`vercel.json`의 rewrite로 루트(`/`)가 `index-classlog.html`로 열립니다.

## 참고

- AI 분석 장치(`clarinet-ai`)는 현재 로컬(PC)에서 실행되는 Python 앱이며, 온라인 웹 버전은 준비 중입니다.
- 데이터는 현재 브라우저 localStorage에 저장됩니다(방·미션). 다중 사용자 공유는 이후 서버/DB 연동이 필요합니다.
