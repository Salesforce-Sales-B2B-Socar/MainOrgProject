# 🏢 Account Domain - Agentforce 통합

> **고객 중심 AI**: 모든 비즈니스는 결국 사람과 사람 사이의 관계입니다.

Account Domain은 SOCAR B2B 플랫폼의 고객 관리 핵심으로, Agentforce와 통합되어 고객 360도 뷰를 제공합니다.

---

## 🎯 Account Domain 개요

### 📋 핵심 기능
- **B2B 고객 관리**: 법인 고객 전용 서비스 및 관리
- **계정 분석**: 고객 행동 패턴 및 비즈니스 인사이트
- **관계 매핑**: 복잡한 B2B 관계 구조 시각화
- **위험도 평가**: AI 기반 고객 이탈 예측

### 🤖 Agentforce 통합 포인트

#### 1. 고객 360도 뷰 제공
```
사용자: "ABC 법인 고객 현황을 알려주세요"
Agentforce: "ABC 법인의 종합 현황을 확인해드리겠습니다."
→ Account Analysis Action 실행
Agentforce: "ABC 법인은 현재 활성 고객으로, 월 평균 이용률 85%, 만족도 4.2/5.0입니다. 최근 3개월간 이용량이 20% 증가했습니다."
```

#### 2. 리스크 분석 및 알림
```
Agentforce: "⚠️ XYZ 법인의 이용률이 지난 달 대비 40% 감소했습니다. 고객 관리팀 컨택을 추천드립니다."
```

---

## ⚡ Account Domain Actions

### 🔍 GetAccountStatus
**목적**: 계정 현재 상태 및 핵심 지표 조회

**입력 파라미터**:
- `accountId` (Required): 계정 ID
- `includefinancials` (Optional): 재무 정보 포함 여부

**출력**:
- 계정 기본 정보
- 활성 상태 및 건강도 점수
- 최근 활동 요약
- 위험도 등급

### 📊 AnalyzeAccountTrend
**목적**: 계정별 트렌드 분석 및 예측

**입력 파라미터**:
- `accountId` (Required): 계정 ID
- `periodMonths` (Optional): 분석 기간 (기본 6개월)

**출력**:
- 이용률 트렌드
- 매출 성장률
- 계절성 패턴
- 미래 예측 데이터

### 🎯 GetAccountOpportunities
**목적**: 계정 내 영업 기회 발굴

**입력 파라미터**:
- `accountId` (Required): 계정 ID
- `opportunityType` (Optional): 기회 유형 필터

**출력**:
- 식별된 영업 기회 목록
- 우선순위 점수
- 추천 액션 플랜
- 예상 ROI

---

## 📚 Knowledge Base - Account 관리

### 🏢 B2B 고객 관리 가이드
- **신규 법인 온보딩 프로세스**
- **계약 갱신 및 확장 전략**
- **고객 만족도 관리 방법**
- **B2B 할인 및 혜택 정책**

### 📊 Account Health Scoring
- **건강도 점수 산정 기준**
- **위험 신호 및 대응 방법**
- **고객 세분화 전략**
- **retention 개선 방안**

### 🔄 Account Lifecycle 관리
- **신규 고객**: 온보딩 프로세스
- **성장 고객**: 확장 영업 전략
- **성숙 고객**: 관계 유지 및 만족도 관리
- **위험 고객**: retention 전략

---

## 🧪 테스트 시나리오

### ✅ 성공 시나리오

#### 계정 상태 조회
```
사용자: "SOCAR 파트너스 계정 상태 알려주세요"
Agentforce: 
- 현재 상태: 활성 (Health Score: 85/100)
- 월 이용률: 78% (전월 대비 +5%)
- 활성 주문: 23건
- 만족도: 4.3/5.0
- 다음 갱신일: 2024-12-15
```

#### 위험 고객 알림
```
Agentforce: "⚠️ ABC 건설의 Health Score가 65점으로 하락했습니다.
주요 원인:
- 이용률 20% 감소
- 최근 30일간 문의 3건 증가
권장 액션: 고객 면담 스케줄 예약"
```

### ⚠️ 예외 처리

#### 계정 정보 없음
```
사용자: "존재하지않는회사 정보 알려주세요"
Agentforce: "죄송합니다. 해당 계정을 찾을 수 없습니다. 계정명을 다시 확인해주시거나, 신규 계정 등록이 필요한 경우 영업팀(02-1234-5678)으로 연락주세요."
```

---

## 📊 성능 지표

### 🎯 Account Health Metrics
- **전체 계정 Health Score 평균**: 82/100
- **위험 계정 비율**: 15% 이하 유지
- **계정 성장률**: 월 평균 8%
- **고객 만족도**: 4.2/5.0 이상

### 📈 AI 예측 정확도
- **이탈 예측 정확도**: 87%
- **성장 기회 예측**: 92%
- **갱신 확률 예측**: 89%

---

## 🔗 관련 도메인 연계

### 🔄 Order Domain
- 계정별 주문 패턴 분석
- 주문 기반 고객 세분화

### 💰 Payment Domain  
- 결제 패턴을 통한 신용도 평가
- 계정별 결제 건강도 모니터링

### 🚗 Asset Domain
- 계정별 Asset 이용 최적화
- 차량 배치 및 수요 예측

### 🎯 Opportunity Domain
- Account 기반 영업 기회 창출
- 업셀/크로스셀 기회 식별

---

## 💡 베스트 프랙티스

### 🎯 Account 관리 전략
1. **프로액티브 모니터링**: 위험 신호 조기 감지
2. **개인화된 서비스**: 계정별 맞춤 솔루션 제공
3. **지속적 관계 강화**: 정기적 건강도 체크

### 📊 데이터 품질 관리
1. **정확한 데이터 입력**: 계정 정보 실시간 업데이트
2. **중복 계정 방지**: 데이터 정합성 유지
3. **권한 관리**: 민감 정보 접근 통제

---

**🏢 Account Vibe**: "고객은 숫자가 아닌 사람입니다. 데이터 뒤에 숨은 진짜 이야기를 읽어내세요." 💼
