# Week 1 - 기술 선정

## ✅ 주요 목표
- 각 영역별 기술 후보 조사
- 장단점 비교 후 최종 선택

## 🔑 결정 사항

### 인증/인가 + 웹서버 + WAS
- 후보: Spring Security + JWT, Keycloak, OAuth2 Provider
- 결정: Spring Security + JWT
- 이유: 팀 내 경험도가 높고, 가볍게 시작 가능

### 컨테이너 관리 (CI/CD)
- 후보: Jenkins, GitHub Actions, ArgoCD
- 결정: GitHub Actions
- 이유: GitHub와 연동이 편하고 초기 셋업 간단

### 이벤트 처리
- 후보: RabbitMQ, Kafka
- 결정: Kafka
- 이유: 대용량 이벤트 처리와 추후 확장성 고려

### DB, 캐싱
- 후보: MySQL, PostgreSQL, Redis
- 결정: MySQL + Redis
- 이유: MySQL은 친숙성, Redis는 캐싱과 세션 관리 최적화

### 모니터링 / 로그 수집
- 후보: ELK Stack, Prometheus + Grafana + Loki
- 결정: Prometheus + Grafana + Loki
- 이유: 경량화된 모니터링, 클라우드 친화적
