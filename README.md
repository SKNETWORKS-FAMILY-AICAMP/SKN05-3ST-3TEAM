# SKN05-3RD-3TEAM

### 🤖 3차 프로젝트: LLM 기반 내외부 기반 질의응답 시스템  
**프로젝트명:** 법률 확인 챗봇 시스템  
**개발기간:** 2024.11.26 - 2024.11.27  

## 💻 팀 소개

**팀명:** 보람3조  

| **김요은👩‍💻** | **박찬규👨‍💻** | **김혜서👩‍💻** | **박보람👩‍💻** |
|:--------------:|:--------------:|:--------------:|:--------------:|
| @usey10        | @thanGyuPark   | @Hyeseo20      | @pbr2858        |

---

### 📌 1. 프로젝트 개요

#### 1.1. 개발 동기 및 목적  
현재 실생활에서 접할 수 있는 챗봇은 고객을 위한 챗봇입니다.  
하지만 본 프로젝트는 **기업의 원활한 업무를 위한 챗봇**을 구현하고자 했습니다.  
특히 **인사, 징계, 복무 규정** 등 기업의 중요한 법적 규정을 챗봇을 통해 **정확히 안내**할 수 있도록 구현했습니다.  
외부 문서로는 **대한민국 헌법**을 바탕으로, **AI HUB의 법률/규정 텍스트**를 활용하여 법률과 규정에 대해 응답할 수 있는 챗봇 시스템을 개발했습니다.  

#### 1.2. 필요성  
일반적인 챗봇은 특정 기업에 대한 정보가 부족하여, 통상적인 정보만을 제공합니다.  
특히, **공항과 같은 특수 시설**에서 적용되는 규정들이 있으므로, 해당 규정들을 학습시켜, **정확하고 구체적인 정보**를 제공할 필요가 있었습니다.

#### 1.3. 개발 목표  
- **특화된 정보 제공:** 공항 및 관련 기관의 규정과 절차를 반영한 답변 제공  
- **정확성 향상:** 일반적인 챗봇 한계를 넘어, **정확하고 구체적인 답변** 제공  
- **사용자 경험 개선:** 직관적이고 빠른 정보 제공을 위한 **UI/UX 최적화**  

---

### 📌 2. 기술 스택

#### 2.1. 프론트엔드
<div>
<img src="http://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=Streamlit&logoColor=white"> 
</div> 

#### 2.2. 백엔드
<div>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"> 
</div> 
- 오픈AI, 랭체인, pypdfloader를 사용하여 백엔드 처리 예정

---

### 📌 3. WBS (Work Breakdown Structure)

#### 3.1. 내부 데이터 수집 및 전처리
- 한국 공항 공사 **인사, 복무, 징계** 규정 다운로드  
- HTML 태그, URL 등 **불필요한 정보 제거**  

#### 3.2. 외부 데이터 수집 및 전처리
- **AI HUB** 법률/규정 텍스트 데이터 다운로드  
- **불필요한 판결문 제거**  

#### 3.3. API 사용하여 GPT 모델 파인 튜닝
- **토큰 수 계산 및 비용 산정**  
- **GPT 모델 선정** 및 결과 비교  

#### 3.4. RAG 구현
- **파인튜닝 모델 사용**  
- **답변 검증 및 비교**  

#### 3.5. STREAMLIT 구현

---

### 📌 4. 모델 별 답변 비교 & 검증

#### 4.1. 모델 별 답변 비교 예시

| **질문** | **기본 GPT 모델** | **벡터 스토어** | **파인 튜닝** | **파인 튜닝 + 벡터 스토어** | **규정 내용 확인** |
|:--------:|:----------------:|:--------------:|:------------:|:-------------------------:|:-----------------:|
| 감봉 사유 | 직무 관련 의무 위반, 명령 불이행 등 | 감봉 사유를 구체적으로 나열 | 감봉 사유를 직무 관련으로 설명 | 다양한 사유를 상세히 나열 | 문서 상에서 구체적 사유 제공 |

---

### 📌 5. 답변 검증

#### 5.1. 답변 검증 예시

| **공무직 근로자 관리 예규** | **안전사고예방 근로자 문책규정** | **인사 규정** |
|:---------------------------:|:-----------------------------:|:------------:|
| **징계의 종류** 파면, 해임, 정직, 감봉 등 명시 | **징계 종류 및 효과** 경고, 주의 등 명시 | **징계 사유** 직무 의무 위반 등 명시 |

---

### 📌 6. STREAMLIT 구현 결과
- 프로젝트의 주요 기능과 모델을 **Streamlit**으로 구현하여, 직관적인 사용자 인터페이스를 제공

---

### 📌 7. 한 줄 회고

• 김요은:
• 박찬규: 
• 김혜서: 
• 박보람: 

