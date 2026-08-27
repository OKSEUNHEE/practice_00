# 주식성향 테스트

## 기능 개요

투자자의 투자 기간, 손실 감내 수준, 변동성 선호도와 투자 점검 습관을 확인해 학습용 투자 성향을 안내하는 기능입니다.

## 제공 성향

- 안정 추구형
- 균형형
- 성장 추구형
- 적극 투자형

## 사용 방법

1. 공통 메뉴에서 `투자성향 테스트`를 선택합니다.
2. 6개 문항에 현재 투자 성향과 가까운 답을 선택합니다.
3. `결과 확인`을 눌러 점수와 성향별 학습 가이드를 확인합니다.

테스트 응답은 브라우저의 `localStorage`에 저장되어 새로고침 후에도 유지됩니다.

## 변경 파일

- `frontend/js/analysis.js`: 문항, 점수 계산, 결과 렌더링, 응답 저장
- `frontend/css/analysis.css`: 질문 및 결과 화면 스타일
- `frontend/js/common.js`: 공통 메뉴의 독립 `투자성향 테스트` 링크
- `frontend/analysis.html`: 공통 스크립트 캐시 버전 갱신
- `frontend/trade/stock.html`: 공통 스크립트 캐시 버전 갱신

## 확인 주소

```text
http://localhost:3000/analysis.html?lesson=stock-personality
```

모든 결과는 교육용 자기 점검이며 투자 권유가 아닙니다.

## Git 기록

- Commit: `98debf6 Add stock personality test`
- Remote: `origin/main`
- 운영 배포 workflow는 `STOCK_TRADE_DEPLOY_TOKEN` 설정이 필요합니다.
