## 안녕하세요! 👋 Backend 개발자 김태영입니다

Java/Spring Boot 기반 백엔드 개발자로, AI, 블록체인, 실시간 통신 기술을 활용한 다양한 프로젝트 경험이 있습니다.

**Email**: erd57819@gmail.com

---

### 🛠 Tech Stack

**Backend**

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white)
![QueryDSL](https://img.shields.io/badge/QueryDSL-4479A1?style=flat-square&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

**Database & Infra**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

**DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Zustand](https://img.shields.io/badge/Zustand-764ABC?style=flat-square&logoColor=white)

**Blockchain & AI**

![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=flat-square&logo=ethereum&logoColor=white)
![Web3j](https://img.shields.io/badge/Web3j-F16822?style=flat-square&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)

---

### 📂 Projects

#### 1. Yammy - 야구 팬 올인원 플랫폼 `2025.10 ~ 2025.11`

**GitHub**: [Yammy](https://github.com/erd57819/Yammy)

**담당 역할**: Backend (NFT 블록체인, 소셜 로그인, SNS 기능)

**핵심 구현**
- **NFT 블록체인 티켓**: Ethereum Sepolia + IPFS 연동, 3단계 에러 복구로 발급 성공률 99% 달성, 발급 시간 65% 단축
- **카카오 OAuth 2.0**: 소셜 로그인으로 회원가입 전환율 40% 향상, 가입 시간 120초→8초 단축
- **SNS 팔로우 시스템**: Idempotent API + 무한 스크롤로 로딩 시간 70% 단축 (3초→1초)

**기술 스택**: `Spring Boot` `React` `Web3j` `Ethereum` `IPFS` `Redis` `Kafka` `AWS S3`

---

#### 2. LastDance - 블록체인 유언장 공증 서비스 `2025.09 ~ 2025.10`

**GitHub**: [LastDance](https://github.com/erd57819/LastDance)

**담당 역할**: Frontend (WebRTC 화상 공증, 결제 시스템, UI/UX)

**핵심 구현**
- **LiveKit WebRTC 화상 공증**: OpenVidu→LiveKit 마이그레이션으로 연결 안정성 85% 개선 (실패율 35%→5%)
- **공증예약 시스템**: Kakao Map API 연동 + 주소 검색 정확도 60%→95% 향상, 검색 응답 80% 개선
- **Toss Payments 결제**: 결제 성공률 85%→95% 향상, 자동 롤백으로 환불 요청 90% 감소

**기술 스택**: `Spring Boot` `React` `LiveKit` `PostgreSQL` `Ethereum` `IPFS` `Toss Payments` `Modusign`

---

#### 3. Dochi (참견도치) - AI 갈등 해결 서비스 `2025.07 ~ 2025.08`

**GitHub**: [Dochi](https://github.com/erd57819/Dochi)

**담당 역할**: Backend/AI (실시간 감정 분석, AI 코칭 시스템)

**핵심 구현**
- **실시간 AI 코칭**: 6가지 감정 트리거 패턴 설계, 코칭 응답시간 3초→1초 (70% 단축)
- **한국어 감정 분석**: Google Cloud NLP + 키워드 패턴으로 감정 분석 정확도 45%→75% 개선
- **AI API 비용 최적화**: 프롬프트 토큰 35% 절감으로 월 운영비 30% 절감 ($180→$126)

**기술 스택**: `Spring Boot` `FastAPI` `React` `Claude AI` `Google Cloud NLP` `Redis` `Docker`

---

#### 4. Cu-Link - LLM 뉴스 리포트 자동화 서비스 `2024.10 ~ 2025.07`

**GitHub**: [Cu-Link](https://github.com/erd57819/Cu-Link)

**담당 역할**: Fullstack (뉴스 크롤링 자동화, AI 요약, 세션 관리, 기사 CRUD)

**핵심 구현**
- **뉴스 크롤링 자동화**: Selenium WebDriver + 페이지네이션으로 6개 필드 자동 수집, Set 기반 중복 필터링으로 데이터 정확도 95% 달성
- **벡터 검색 시스템**: SentenceTransformer(all-MiniLM-L6-v2) + FAISS IndexFlatL2로 유사 기사 시맨틱 검색 구현
- **데이터 분산 저장**: MySQL 메타데이터 + Firebase 원문 JSON 분리 저장으로 조회 속도 60% 개선
- **AI 기사 요약**: OpenAI GPT + Firebase 연동, 다중 기사 병렬 처리로 요약 시간 85% 단축

**기술 스택**: `Node.js` `Express` `FastAPI` `React` `MySQL` `Firebase` `OpenAI API` `LangChain` `Selenium` `FAISS`

---


### 💡 핵심 역량

**Backend**
- Spring Boot, JPA/QueryDSL, Spring Security, JWT 인증
- Web3j, Ethereum, 스마트 컨트랙트 연동
- IPFS (Pinata), OAuth 2.0 소셜 로그인
- Redis 캐싱, Kafka 메시지 큐

**Frontend**
- React, Zustand 상태 관리
- WebRTC (LiveKit), 무한 스크롤
- 반응형 디자인, Protected Routes
