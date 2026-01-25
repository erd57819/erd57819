## 안녕하세요! 👋 Backend 개발자 김태영입니다

Java/Spring Boot 기반 백엔드 개발자로, AI, 블록체인, 실시간 통신 기술을 활용한 다양한 프로젝트 경험이 있습니다.

📧 **Email**: erd57819@gmail.com

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

#### 1. Dochi (참견도치) - AI 갈등 해결 서비스
> 실시간 감정·대화 분석을 통한 AI 갈등 해결 서비스

**GitHub**: [Dochi](https://github.com/erd57819/Dochi) | **담당 역할**: Backend (AI 연동, 실시간 통신)

| 항목 | 내용 |
|------|------|
| AI 갈등 레포트 | 고민을 유형·상황·목표별로 분석하고 책임 비율 제시 |
| 실시간 대화 코칭 | 화상통화 중 표정+음성 감정 분석으로 AI 중재 |
| 토닥토닥 챗봇 | 고민 상담 특화 모델로 위로와 조언 제공 |

**기술 스택**: `Spring Boot` `FastAPI` `React` `GPT-4/Claude` `WebRTC` `Redis` `Kafka` `Docker`

---

#### 2. Yammy - 야구 팬 올인원 플랫폼
> 경기 정보, AI 승부예측, 실시간 응원채팅, NFT 티켓, 중고 굿즈 거래

**GitHub**: [Yammy](https://github.com/erd57819/Yammy) | **담당 역할**: Backend (NFT 블록체인, 소셜 로그인, SNS 기능)

| 항목 | 개선 전 | 개선 후 | 개선율 |
|------|---------|---------|--------|
| NFT 발급 에러율 | 15% | 0.3% | **98% 감소** |
| NFT 발급 시간 | 12초 | 4.2초 | **65% 단축** |
| 회원가입 전환율 | 60% | 85% | **40% 향상** |
| SNS 초기 로딩 | 3.2초 | 0.96초 | **70% 단축** |

**핵심 구현**
- **NFT 블록체인 티켓**: Ethereum Sepolia + IPFS 연동, 멱등성 설계로 가스비 100% 절감
- **카카오 OAuth 2.0**: 원클릭 로그인, JWT 토큰 자동 발급, 탈퇴 회원 재가입 방지
- **SNS 팔로우 시스템**: Idempotent API 설계로 중복 요청 에러 100% 제거

**기술 스택**: `Spring Boot` `FastAPI` `React` `GPT-4` `Web3j` `Ethereum` `IPFS` `Redis` `Kafka`

---

#### 3. LastDance - 블록체인 유언장 공증 서비스
> 디지털 유언장 작성, 화상 공증, 블록체인 기록

**GitHub**: [LastDance](https://github.com/erd57819/LastDance) | **담당 역할**: Frontend (WebRTC 화상 공증, 결제 시스템, UI/UX)

| 항목 | 개선 전 | 개선 후 | 개선율 |
|------|---------|---------|--------|
| WebRTC 연결 실패율 | 35% | 5% | **86% 개선** |
| 결제 승인 성공률 | 85% | 98% | **15% 향상** |
| 회원가입 완료율 | 60% | 82% | **37% 향상** |
| 모바일 이탈률 | 40% | 18% | **55% 감소** |

**핵심 구현**
- **LiveKit WebRTC 화상 공증**: 491줄 커스텀 훅 설계, 4인 동시 화상통화 및 녹화
- **공증예약 시스템**: 191개 더미 데이터 제거 및 DB 연동, 검색 응답 80% 개선
- **Toss Payments 결제**: 결제 실패 시 자동 롤백, 환불 요청 90% 감소

**기술 스택**: `Spring Boot` `React` `LiveKit` `PostgreSQL` `Ethereum` `IPFS` `Toss Payments` `Modusign`

---

#### 4. Cu-Link - LLM 뉴스 리포트 자동화 서비스
> 키워드 기반 뉴스 검색 및 AI 요약 리포트 생성

**GitHub**: [Cu-Link](https://github.com/erd57819/Cu-Link) | **담당 역할**: Fullstack (AI 요약, 세션 관리, 기사 CRUD)

| 항목 | 개선 전 | 개선 후 | 개선율 |
|------|---------|---------|--------|
| 프론트엔드 리소스 | 1.04MB | 0.07MB | **93% 절감** |
| 컴포넌트 코드량 | 87줄 | 60줄 | **31% 감소** |
| API 응답 시간 | 전체 조회 | 페이지네이션 | **75% 단축** |
| 기사 요약 시간 | 수동 읽기 | AI 요약 | **85% 단축** |

**핵심 구현**
- **AI 요약 기능**: OpenAI GPT 모델 연동, Firebase Storage에서 원문 조회 후 자동 요약
- **MySQL 세션 관리**: 서버 재시작 시에도 세션 유지율 100% 달성
- **기사 CRUD**: 중복 저장 방지, 권한 검증 기반 삭제 기능

**기술 스택**: `Node.js` `Express` `FastAPI` `React` `MySQL` `Firebase` `OpenAI API` `LangChain`

---

### 📊 GitHub Stats

![erd57819's GitHub stats](https://github-readme-stats.vercel.app/api?username=erd57819&show_icons=true&theme=default)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=erd57819&layout=compact)

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

**DevOps & Infra**
- Docker, Jenkins CI/CD, AWS EC2/S3
- Nginx, GitLab CI/CD

---

### 📫 Contact

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/erd57819)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:erd57819@gmail.com)
