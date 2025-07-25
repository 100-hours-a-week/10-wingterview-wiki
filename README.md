# 10-team-matching_quiz-wiki
10조 모의면접 매칭 및 퀴즈 서비스 Wiki
<div align="center">
  <img src="https://github.com/user-attachments/assets/fcbe381a-189e-4d70-ac82-722e12acfd9c" alt="Logo" width="100" >
  <h1>Wingterview</h1>
  <p>
    <a href="https://wingterview10.com">서비스 바로가기</a> <br>
    <a> Wingterview는 평일 13:00 ~ 19:00까지 운영합니다!</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details align="left">
  <summary>Table of Contents</summary>
    <div><a href="#프로젝트-소개">프로젝트 소개</a></div>
    <div><a href="#mvp-발전-과정">MVP 발전 과정</a></div>
    <div><a href="#주요-기능">주요 기능</a></div>
    <div><a href="#팀원-소개">팀원 소개</a></div>
    <div><a href="#기술-스택">기술 스택</a></div>
    <div><a href="#개발-일정">개발 일정</a></div>
    <div><a href="#아키텍처-구조">아키텍처 구조</a></div>
    <div><a href="#api-명세서">API 명세서</a></div>
</details>

# 📖 프로젝트 소개

### 프로젝트 이름

윙터뷰 (Wingterview), 면접에 날개를 달자! 🪽

### 프로젝트 기간

2025.03.31 ~ 2025.08.01

### 프로젝트 설명

윙터뷰는 개발자 취업을 준비하는 사람들을 위한 AI 면접 훈련 플랫폼입니다.
사용자가 직무와 기술 스택을 입력하면, AI가 맞춤형 질문을 제시하고 사용자는 음성으로 답변합니다.
이후 사용자가 간단한 키워드나 피드백을 입력하면,
AI가 이를 바탕으로 꼬리질문을 생성해 심화 면접처럼 이어집니다.
면접이 끝나면, AI는 피드백과 모범답안, **복습 퀴즈(CS 포함)** 를 제공해 반복 학습을 지원합니다.

> 윙터뷰는 초창기 **1차 MVP** 단계에서 카카오테크 부트캠프 수강생을 위한  
> **실시간 1:1 매칭 기반 모의면접 서비스**로 시작되었습니다.  
> 그러나 전체 교육생 및 일반 취업 준비생을 대상으로 서비스 범위를 확장하며,  
> **시간 제약 없이 누구나 반복 학습 가능한 AI 기반 면접 시스템**이 더 효과적이라는 판단에 따라  
> 현재의 **2차 MVP**에서는 **AI와 함께하는 나홀로 면접 방식으로 전환**하게 되었습니다.

---

> ### 윙터뷰🪽는 이런 사람들에게 필요해요!
>
> ✔️ 면접관 없이 혼자서 실전처럼 기술 면접을 연습하고 싶은 사람  
> ✔️ 답변에 대한 **즉각적인 피드백과 모범답안** 이 필요한 사람  
> ✔️ 반복적인 면접 훈련을 통해 실력을 꾸준히 쌓고 싶은 사람  
> ✔️ 다른 사람들의 답변을 보고 함께 학습하고 싶은 사람  
> ✔️ 면접 내용을 기반으로 한 복습 퀴즈와 CS 지식을 병행 학습하고 싶은 사람

---

## 🚀 릴리즈 노트

### ✅ 1차 MVP 요약 (2025.05 기준)

- **운영 시간**: 월, 화, 수 10:00 ~ 12:00  
- **매일 9:50**에 **자동 1:1 실시간 매칭** 시작  
- **핵심 컨셉**: 카카오테크 부트캠프 수강생(취준생)을 위한 **1:1 모의면접 도우미 및 자동 매칭 서비스**

| 기능 번호 | 기능명               | 설명                                   |
|-----------|----------------------|----------------------------------------|
| 1         | 카카오 로그인        | 직무, 기술스택 입력 기반 온보딩       |
| 2         | 1:1 실시간 매칭     | 매일 9:50 랜덤 매칭 → 역할 교대       |
| 3         | AI 면접 질문 생성   | 직무/스택 기반 기술 면접 질문         |
| 4         | 나홀로 모의면접(예정) | 녹음 → AI 피드백 제공                  |
| 5         | 복습 퀴즈 제공(예정) | 면접 내용 기반 퀴즈 생성               |

---

### ✅ 2차 MVP 요약 (2025.06 기준)

- **운영 시간**: **월~금 13:00 ~ 20:00**  
- **상시 면접 시작 가능** (자동 매칭 없음)  
- **핵심 컨셉**: 개발자로 취업하고자 하는 취준생을 위한 AI 기반 **기술 면접 훈련 플랫폼**

| 기능 번호 | 기능명            | 설명                                               |
|-----------|-------------------|----------------------------------------------------|
| 1         | 카카오 로그인     | 직무/스택 기반 온보딩                             |
| 2         | 나홀로 AI 면접   | AI 질문 → 음성 답변 → 피드백 + 모범답안           |
| 3         | AI 면접 질문 생성 | 맞춤형 기술 질문 생성                              |
| 4         | 복습 퀴즈         | 응답 기반 퀴즈 + CS 퀴즈 제공                      |
| 5         | 게시판 커뮤니티   | 모범답안 공유 및 토론 기능 신설                    |

---

### 🔄 주요 변경 사항 요약

| 항목              | 1차 MVP                             | 2차 MVP                                           |
|-------------------|--------------------------------------|--------------------------------------------------|
| **매칭 방식**     | 실시간 자동 매칭 (사람 간 1:1)       | AI 기반 나홀로 면접                              |
| **운영 시간**     | 월~수 10:00 ~ 12:00                  | 월~금 13:00 ~ 20:00                              |
| **AI 피드백**     | 예정 기능                            | 정식 제공 (모범답안 + 피드백제공)                    |
| **복습 퀴즈**     | 예정 기능                            | 정식 제공 (면접 기반 + CS 퀴즈)                  |
| **게시판 기능**   | 없음                                 | 신설 (답안 공유, 토론 가능)                      |

---

## 👥 팀원 소개

<table>
<thead>
  <tr>
    <th align="center">🩷팀장🩷 AI</th>
    <th align="center">AI</th>
    <th align="center">AI</th>
    <th align="center">FRONTEND</th>
    <th align="center">BACKEND</th>
    <th align="center">CLOUD</th>
    <th align="center">CLOUD</th>
  </tr>
</thead>
  <tr>
    <th align="center"><a href="https://github.com/sde00">eunice.song</a></th>
    <th align="center"><a href="https://github.com/tykong08">tommy.kong</a></th>
    <th align="center"><a href="https://github.com/chan-980730">david.lee</a></th>
    <th align="center"><a href="https://github.com/devjoylee">joy.lee</a></th>
    <th align="center"><a href="https://github.com/imleokkkk">leo.kim</a></th>
    <th align="center"><a href="https://github.com/year99">ken.kim</a></th>
    <th align="center"><a href="https://github.com/kim-jihoo">jihoo.kim</a></th>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/sde00">
        <img src="https://avatars.githubusercontent.com/sde00" width="100px;" heightalt="" />
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/tykong08">
        <img src="https://avatars.githubusercontent.com/tykong08" width="100px;" alt="" />
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/chan-980730">
        <img src="https://avatars.githubusercontent.com/chan-980730" width="100px;" alt="" />
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/devjoylee">
        <img src="https://avatars.githubusercontent.com/devjoylee" width="100px;" alt="" />
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/imleokkkk">
        <img src="https://avatars.githubusercontent.com/imleokkkk" width="100px;" alt="" />
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/year99">
        <img src="https://avatars.githubusercontent.com/year99" width="100px;" alt="" />
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/kim-jihoo">
        <img src="https://avatars.githubusercontent.com/kim-jihoo" width="100px;" alt="" />
      </a>
    </td>
  </tr>
</table>

<br>

## 🛠 기술 스택

### 프론트엔드 

기술 영역 | 선택한 기술 | 선택 이유 및 장점
-- | -- | --
FE 프레임워크 | `React`(v19) + `Typescript`(v.5) + `Vite`(v6) | - 동적 상호작용이 많은 CSR 위주 서비스에 최적화 <br/> - React 동시성기능 + Vite의 빠른 빌드 = 사용자경험 향상
상태 관리 | `Zustand` (v5.0.3) | - Context API 대비 불필요한 리렌더링 감소로 성능 향상 <br/>  - Redux보다 낮은 학습 곡선 + 간결한 API
스타일링 | `CSS Modules` + `SCSS` | - 스타일링 커스텀의 자유도가 높음. 스타일 컴포넌트화 <br/>  - Sass의 변수, 믹스인, 중첩 규칙 등 활용 가능
폼 관리 | `React Hook Form` (v.7.50.0) | - 불필요한 리렌더링 최소화로 성능 최적화 <br/>  - 폼 유효성 검증 & 상태 관리 편리함
Data Fetching | `Tanstack Query` (v.5.36.0) | - 서버 상태 관리 및 자동 캐싱 기능 <br/>  - 데이터 상태(로딩, 에러, 성공) 관리 간소화 

### AI

기술 영역 | 선택한 기술 | 선택 이유 및 장점 
-- | -- | --
개발 언어 | `Python`(3.11.12) | - 주요 컴포넌트 기반 언어<br>-빠른 서버 개발 및 AI 모델 서빙 최적화 지원
AI 서버 및 서빙 | `FastAPI`(0.115.9) + `vLLM`(0.8.4) | - 경량, 고성능 API 서버(FastAPI)로 API 요청 관리<br>- vLLM 기반 초고속 LLM 추론 서빙 (PagedAttention 활용)<br>- 대규모 동시 요청 처리에 최적화 
체인 구성 및 관리 | `LangChain`(0.3.24) | - 프롬프트, 메모리, 체인 구성 등 모듈화된 구성 지원<br>- 복잡한 LLM 워크플로우 관리 최적화 
벡터 데이터베이스 | `ChromaDB`(1.0.7) | - 빠른 벡터 검색 및 간편한 통합 지원<br>- 서버리스 및 온프레미스 환경 모두 대응 가능 
LLM 평가 및 모니터링 | `LangSmith`(0.3.33) + `Langfuse`(2.60.3) | - LangChain 체인/Agent 성능 모니터링 (LangSmith)<br>- 실시간 응답 품질 및 트레이스 기반 상세 모니터링 (Langfuse)<br>- 사용자 행동/실패율/지연시간 통합 추적 가능 
사전학습 모델 소스 | `Hugging Face Transformers`(4.51.3) | - 최신 llm 모델 지원<br>-vllm과 연동 호환성



<br>

## 🗓 개발 일정

| 기간          | 주요 작업               |
| ------------- | ----------------------- |
| 03/31 ~ 04/13 | 서비스 기획             |
| 04/14 ~ 04/27 | 디자인 및 설계          |
| 04/28 ~ 05/11 | MVP 개발                |
| 05/12 ~ 05/18 | 1차 배포 및 출시        |
| 05/19 ~ 05/25 | 서비스 홍보 및 유지보수 |
| 05/26 ~ 06/15 | 업데이트 개발           |
| 06/16 ~ 06/22 | V2 업데이트             |
| 06/23 ~ 06/29 | 유지보수                |
| 06/30 ~ 07/06 | 업데이트 개발           |
| 07/07 ~ 07/13 | V3 업데이트             |
| 07/14 ~ 07/20 | 유지보수                |
| 07/21 ~ 07/27 | 업데이트 개발           |
| 07/28 ~ 08/01 | V4 업데이트             |

<br>

## 🧩 아키텍처 구조

> (아키텍처 이미지 혹은 도식 첨부 예정)

<br>

