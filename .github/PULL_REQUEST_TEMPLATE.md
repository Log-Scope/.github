<!--
LogScope PR 제목 규칙(필수)
- feat|fix|chore|docs|refactor|test|perf|ci|build: 요약 (#이슈번호)
예) feat: 로그 수집 파이프라인(OTel → Loki) 추가 (#12)
예) fix: 검색 결과 정렬 불일치 수정 (#34)

기본 원칙
- 한 PR = 한 목적
- 본문에 반드시 `Closes #번호`(또는 Fixes/Resolves)로 이슈 연결
- 머지 시 자동으로 이슈 닫히게 하려면: PR 본문에 키워드 + 이슈번호를 적어야 함
-->

## 구현 내용
- 

## 구현 이유 / 배경
- 

## 변경 사항 요약 (Diff)
- (추가/수정/삭제한 핵심만 3줄 이내)
- 

## 영향 범위 (체크)
- [ ] Ingestion (수집/에이전트)
- [ ] Parsing/ETL (파싱/정규화)
- [ ] Storage (저장/인덱싱)
- [ ] Search/API (검색/조회 API)
- [ ] UI/Console (대시보드/콘솔)
- [ ] Alerting (알림/룰)
- [ ] Ontology/Schema (온톨로지/스키마)
- [ ] Auth/Org (권한/테넌시)
- [ ] Infra/Deploy (배포/인프라)

## Breaking / Migration 체크
- [ ] Breaking change 있음 (사용자/서비스 영향)
- [ ] Migration 필요 (DB/인덱스/설정)
  - 내용:
  - 롤백 방법:

## 확인 방법 (테스트/검증)
- [ ] 로컬에서 직접 확인함
- [ ] 단위 테스트 추가/수정
- [ ] 통합 테스트/수동 시나리오 검증
- [ ] 로그/스크린샷 첨부 (필요 시)
- 재현/검증 절차:
  1) 
  2) 

## 이슈 자동 종료 (Auto-close)
<!--
머지(merge) 시 이슈가 자동으로 닫히는 키워드:
- close, closes, closed
- fix, fixes, fixed
- resolve, resolves, resolved

✅ 아래 줄을 채우면 PR이 머지될 때 이슈가 자동으로 닫힘
- Closes #123
- Fixes #123
- Resolves #123

여러 개 닫기:
- Closes #123, #124
또는
- Closes #123
- Closes #124
-->
- Closes #

## 성능/운영 영향 (선택)
- [ ] 쿼리/인덱싱 성능 영향 있음
- [ ] 비용/리소스 영향 있음 (CPU/Mem/Storage)
- 메모:
  - 

## 보안/권한 (선택)
- [ ] 권한/테넌시 관련 변경
- [ ] 민감정보(PII/Secret) 처리 변경
- 메모:
  - 
