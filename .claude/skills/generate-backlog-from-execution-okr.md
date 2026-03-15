# Skill: Execution OKR Backlog Generator

## 목적

Execution OKR을 입력받아
Frontend / Backend Backlog Title을 생성한다.

---

# 입력

Execution OKR Table

예

| O | K | R |
|---|---|---|
| 트렌드 기반 콘텐츠 노출 전략 실험 | CTR, SR 변화 관찰 | CTR 계산 |

---

# 생성 규칙

Backlog 생성은 다음 절차를 따른다.

1. Execution O에서 핵심 행동을 추출한다
2. 행동을 Frontend / Backend 책임으로 분리한다
3. K, R 지표를 이벤트 수집 행동으로 변환한다
4. Actor + 행동 + 대상 구조로 Backlog Title을 생성한다

---

# Actor 규칙

Frontend

애플리케이션  
추천 페이지  
콘텐츠 페이지

Backend

백엔드 서버  
API 서버  
시스템

---

# 출력 형식

Frontend Backlog Titles

Behavior Backlog

- ...

UI Backlog

- ...

Backend Backlog Titles

Behavior Backlog

- ...