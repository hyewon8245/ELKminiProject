# ELKminiProject
FISA학생들의 스터디 활성화를 위한 데이터분석 미니 프로젝트입니다

## 팀원
<table>
  <tr>
    <th>이용훈</th>
    <th>홍혜원</th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/dldydgns.png" width="120" /><br/>
      <a href="https://github.com/dldydgns">@이용훈</a>
    </td>
    <td align="center">
      <img src="https://github.com/hyewon8245.png" width="120" /><br/>
      <a href="https://github.com/hyewon8245">@홍혜원</a>
    </td>
  </tr>
</table>





## 🔍 ELK 스터디 개요: 출석 및 취향 기반 데이터 분석

### 1. ✅ 스터디 목적

- **ELK 스택의 실습 중심 학습**: 실데이터를 이용해 Elasticsearch, Logstash, Kibana의 연동과 기능을 체험
- 현재 출석데이터를 자동화기능을 사용해서 ELK에 탑재해 분석하는 시스템 개발
- 현재, 비슷한 취향, 취미 등을 가진 친구들을 분석
- 훗날 모인 데이터를 통해 지각하는 사람들의 특성을 분석하고자 하는 기본 분석시스템 개발

---

### 2. 📊 사용 데이터

- **출석 현황** :  날짜별 출석 여부, 지각/결석 여부
- 훈련생정보 : 기본프로필, MBTI, 싫어하는 것. 좋아하는 것, 희망하는 직업분야,

---

### 3. ⚙️ 기술 스택

- **Logstash**: CSV의 출석 및 취향 데이터 수집 및 정제
- **Elasticsearch**: 데이터 색인 및 질의, 집계 처리
- **Kibana**: 대시보드 구성 및 시각화
- **(선택)** 간단한 Python Script: 추천 알고리즘 또는 필터 처리용

---

### 4. 🧠 분석/활용 포인트

- **출석률 순위 및 변화 추이 시각화**
- **요일/시간대별 출석 패턴 분석**
- **학생별 취향 분포 시각화**
- **출석률과 취향 간의 상관관계 분석**

---

### 5. 📈 구현 예시 (Kibana 대시보드)

- 출석률 추이 그래프
- 관심사 분포 파이차트
- 출석률 Top/Bottom 5 리스트
- "나랑 비슷한 취향 가진 친구" 리스트

---

### 6. 🔄 느낀 점 및 한계

- 작은 데이터셋으로도 ELK의 시각화 효과를 직관적으로 확인 가능
- Kibana의 집계/필터 기능으로 분석 흐름이 쉬움
- 단순 알고리즘(코사인 유사도, 공통 선택 항목 기반 추천)과의 연계 가능성 탐색
- 복잡한 ML 추천엔 Elasticsearch alone으로 한계가 있음 → 향후 확장 아이디어

---

### 7. 🔜 다음 단계 제안

- 로그 데이터 등 비정형 데이터도 연동해보기
- Beats 활용한 실시간 출석 데이터 수집 실험
- Elasticsearch의 k-NN 기능을 이용한 유사도 기반 추천 고도화
