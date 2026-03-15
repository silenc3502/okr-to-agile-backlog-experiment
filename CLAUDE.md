# CLAUDE.md

# OKR to Backlog Transformation Rules

이 시스템은 Execution OKR을 기반으로
Frontend / Backend / Data Analytics Agile Backlog를 생성한다.

---

# Transformation Principle

Execution OKR은 다음 구조를 가진다.

O = 실행 목표  
K = 관찰 지표  
R = 측정 방식

Execution OKR은 직접 구현 작업이 아니라  
"실험 전략" 또는 "행동 변화 목표"이며,  
측정·분석·지표 계산 관련 행동도 포함된다.

따라서 Backlog 생성 시 다음 변환 과정을 따른다.

Execution OKR  
→ 핵심 행동 추출  
→ 시스템 책임 분리  
→ 이벤트 수집/분석 변환  
→ Actor 기반 Backlog 생성

---

# Step 1 핵심 행동 추출

Execution O에서 시스템이 수행해야 하는 행동을 추출한다.

**예시 Execution O 행동**

- 트렌드 기반 콘텐츠 노출 전략 실험

추출 행동

- 콘텐츠 그룹 분리
- 콘텐츠 노출
- CTR 이벤트 수집
- SR 이벤트 수집
- A/B 실험 수행

---

# Step 2 시스템 책임 분리

행동을 다음 시스템으로 분리한다.

**Backend 책임**

- 데이터 수집
- 콘텐츠 그룹 분류
- 실험 그룹 할당
- 이벤트 저장

**Frontend 책임**

- 콘텐츠 표시
- 사용자 인터랙션 처리
- 이벤트 트래킹

**Data Analytics 책임**

- 지표 계산 (CTR, SR, EAI, LOI, MCI, SHI 등)
- 통계적 검정 및 실험 분석
- 초기 신호 감지 및 시차 분석
- 실험 그룹 비교 및 전략 평가

---

# Step 3 이벤트/지표 변환

K 또는 R에 포함된 지표는  
항상 이벤트 수집 또는 계산 행동으로 변환한다.

**예시 K/R 지표 변환**

- CTR → 클릭 이벤트
- SR → 전환 이벤트
- LOI → 상태 이벤트

---

# Step 4 Backlog Title 생성 규칙

Backlog Title은 다음 구조를 따른다.

**Backlog Title 구조**

- Actor + 행동 + 대상

Actor는 다음 중 하나여야 한다.

**Frontend**

- 애플리케이션
- 추천 페이지
- 콘텐츠 페이지

**Backend**

- 백엔드 서버
- API 서버
- 시스템

**Data Analytics**

- Analytics 시스템
- Metric Engine
- Experiment Engine

---

# Backlog Type

**Frontend**

- Behavior Backlog
- UI Backlog

**Backend**

- Behavior Backlog

**Data Analytics**

- Behavior Backlog

---

# 최종 목표

Execution OKR을 입력하면  
다음 결과를 생성한다.

- Frontend Backlog Titles
- Backend Backlog Titles
- Data Analytics Backlog Titles