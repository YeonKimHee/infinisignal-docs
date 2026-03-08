# Changelog

모든 주요 변경 사항을 기록합니다.

---

## [2.0.0] - 2026-03-08

### Added
- **분할매수 전략 동적화** — 직전 매수가 기반 트리거로 전략 정확도 향상
- **OG 메타 태그 + 파비콘** — URL 공유 시 미리보기 카드 지원
- **UI 대개편** — 사이드바 + 포트폴리오/전략 통합 레이아웃
- **가격 알림 유저 분리** — 유저별 텔레그램 DM 발송 (단톡 금지)

### Changed
- 단일 종목 상세 페이지로 통합 (Dashboard/Prices/Backtest/Signals → Detail 탭)
- 코드 숨기기 기능으로 클린 UI 제공

---

## [1.5.0] - 2026-03-07

### Added
- **뉴스 파이프라인 v2** — 종목별 요약, 감성 트렌드, 주가 연동, 이슈 알림
- **뉴스 임베딩 + 클러스터링** — 관련 뉴스 자동 그룹핑
- **DART 공시 수집** — 전자공시 자동 수집 파이프라인
- 뉴스 목록 기본 중요도 필터 (importance >= 0.3)
- 뉴스 정제 상태 60초 자동 폴링

### Fixed
- Gemini maxOutputTokens 2000 → 8192로 증가 (정제 결과 잘림 해결)
- 임베딩 모델을 gemini-embedding-001로 변경
- RSS 한국어 인코딩 깨짐 해결 (EUC-KR/CP949 지원)
- 운영서버 News DB 테이블 자동 생성

---

## [1.0.0] - 2026-02-12

### Added
- 무한매수법 백테스트 엔진
- KIS OpenAPI 연동 (실시간 WebSocket + REST)
- 실시간 가격 모니터링 (PriceHub)
- 종목 검색 및 워치리스트
- 트레이딩 신호 생성 및 표시
- Google OAuth 인증 + JWT
- 텔레그램 봇 연동 (연결 코드 방식)
- Docker Compose 기반 배포
- NGINX + Let's Encrypt SSL
