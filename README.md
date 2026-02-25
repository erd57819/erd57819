## 안녕하세요! 신입 개발자 김태영입니다

Java/Spring Boot 기반 백엔드 개발자로, AI, 블록체인, 실시간 통신 기술을 활용한 다양한 프로젝트 경험이 있습니다.

**Email**: erd57819@gmail.com

---

### Tech Stack

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
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)
![Web3j](https://img.shields.io/badge/Web3j-F16822?style=flat-square&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)

---

### Projects

#### 1. Yammy - 야구 팬 올인원 플랫폼 `2025.10 ~ 2025.11`

**GitHub**: [Yammy](https://github.com/erd57819/Yammy)

**담당 역할**: Backend (NFT 블록체인, 소셜 로그인, SNS 기능) + Frontend (경기 결과 페이지)

**핵심 구현**
- **ERC-721 스마트 컨트랙트**: Solidity `YammyTicketNFT.sol` 직접 작성 (`mintTicket` / `batchMintTickets` / `burnTicket`), `ticketIdToTokenId` + `tokenIdToTicketId` 양방향 매핑으로 O(1) 조회, `require(ticketIdToTokenId[ticketId] == 0)` 온체인 중복 발급 방지, Hardhat optimizer(runs: 200) + Sepolia 배포 자동화
- **NFT 발급 서비스**: Spring Boot `NftService` 사용자 검증 강화 + 3단계 에러 복구로 발급 성공률 99% 달성, 발급 시간 65% 단축, 중복 발급 요청 Idempotent 처리
- **야구 데이터 파이프라인**: Python 300줄 CSV 야구 통계 데이터 DB 일괄 삽입 스크립트, `MatchResultPage` + `MatchList` 컴포넌트 신규 구현(1,054줄) — 날짜 검색 + 팀 대 팀 스코어보드 UI

**기술 스택**: `Spring Boot` `React` `Solidity` `Hardhat` `Web3j` `Ethereum` `IPFS` `Redis` `Kafka` `AWS S3`

---

#### 2. LastDance - 블록체인 유언장 공증 서비스 `2025.09 ~ 2025.10`

**GitHub**: [LastDance](https://github.com/erd57819/LastDance)

**담당 역할**: Frontend 전체 (WebRTC 화상 공증, 결제, 회원 인증, 전자문서, UI/UX)

**핵심 구현**
- **LiveKit WebRTC 화상 공증**: OpenVidu→LiveKit 마이그레이션, 491줄 `useLiveKitWebRTC` 커스텀 훅 설계 (Exponential Backoff 재연결 최대 5회, 브라우저 Autoplay Policy 해결 위해 `<audio>` DOM 동적 생성), 연결 실패율 35%→5% (86% 개선), 라이선스 비용 100% 절감
- **전자문서 무결성 보장**: Modusign 전자서명 API 연동, 예약 데이터 로딩 후 `readOnly` 조건부 적용으로 공증 데이터 임의 수정 방지, 블록체인 트랜잭션 해시·IPFS CID UI 시각화

**기술 스택**: `React` `LiveKit` `PostgreSQL` `Ethereum` `IPFS` `Toss Payments` `Modusign` `Kakao Map API` `Redis`

---

#### 3. Dochi (참견도치) - AI 갈등 해결 서비스 `2025.07 ~ 2025.08`

**GitHub**: [Dochi](https://github.com/erd57819/Dochi)

**담당 역할**: Backend/AI (실시간 감정 분석, AI 코칭 시스템, 커뮤니티 기능)

**핵심 구현**
- **한국어 감정 분석 엔진**: Google Cloud NLP API 점수(-1.0~1.0)만으로는 한국어 간접 표현 분류 불가 → 6가지 감정별 키워드 패턴 + 간접 표현 패턴(`그런데`, `솔직히` 등) + 감탄부호 빈도 복합 분석으로 감정 분류 정확도 45%→73% (28%p 향상), 간접 표현 인식 정확도 85% 달성
- **실시간 AI 코칭 시스템**: 6가지 감정 트리거 패턴 설계 (즉시개입/연속패턴/악화/침묵-부정/장시간침묵/침묵재개), 침묵 시간 기반 트리거 (15초/20초/30초 임계값), `conversation_heat` 기반 동적 코칭 주기 조정 (15~60초)으로 불필요한 AI API 호출 최소화, 코칭 응답시간 3초→1초 개선
- **프롬프트 엔지니어링**: "갈등 해결 코치" → "실시간 대화 분석 코치"로 역할 재정의, 실제 발언 인용 + 구체적 표현 개선 제안 형식 추가, 트리거별 고정 프롬프트 → 범용 상황 분석 프롬프트로 전환
- **GMS AI Dual API**: Spring Boot `GmsAiClient`에서 OpenAI·Anthropic API 분기 처리, 요청 모델 실패 시 `gpt-4o-mini` fallback 자동 전환으로 서비스 가용성 확보

**기술 스택**: `Spring Boot` `FastAPI` `React` `Claude AI` `Google Cloud NLP` `MyBatis` `Redis` `Docker`

---

#### 4. Cu-Link - LLM 뉴스 리포트 자동화 서비스 `2024.10 ~ 2025.07`

**GitHub**: [Cu-Link](https://github.com/erd57819/Cu-Link)

**담당 역할**: Fullstack (FastAPI AI 서버, Node.js 백엔드, 기사 CRUD, 세션 관리)

**핵심 구현**
- **AI 요약 API 구조 개선**: 기사 원문 전체 전송 방식에서 ID만 전송 후 서버가 Firebase에서 직접 fetch하는 구조로 전환, 요청 payload 6개 기사 기준 ~12KB → 수십 바이트 (98% 감소), 병렬 처리로 요약 시간 85% 단축
- **기사 선택 상태관리 최적화**: `Set`(ID만 저장) → `Map`(전체 데이터 저장)으로 전환, 요약·리포트 요청 시 O(n) 배열 탐색 제거 및 `sessionStorage` 의존성 제거
- **데이터 분산 저장**: MySQL 메타데이터 + Firebase 원문 JSON 분리 저장으로 MySQL 조회 부하 최소화, 페이지네이션(6개 단위 LIMIT/OFFSET) 적용으로 초기 로딩 속도 75% 개선
- **뉴스 크롤링 자동화**: Selenium WebDriver로 다음 뉴스 동적 페이지 크롤링, `time.sleep()` 대신 `WebDriverWait` 명시적 대기로 안정성 확보, 새 탭 방식(`window_handles`)으로 6개 필드(제목·본문·날짜·언론사·이미지·URL) 자동 수집, Set 기반 `(제목, 본문)` 튜플 중복 필터링으로 데이터 정확도 95% 달성
- **3중 저장소 동기화 파이프라인**: 크롤링 데이터를 FAISS(벡터 임베딩) · MySQL(메타데이터) · Firebase(원문 JSON) 3개 저장소에 동시 저장, 저장 후 각 저장소 ID 차집합 연산으로 정합성 검증, MySQL UPSERT(`ON DUPLICATE KEY UPDATE`) 패턴으로 재크롤링 시 중복 방지
- **벡터 검색 시스템**: SentenceTransformer(all-MiniLM-L6-v2)로 본문 384차원 임베딩, UUID → SHA256 해싱 → int64 변환으로 FAISS `IndexIDMap + IndexFlatL2` 호환, L2 거리 기반 유사 기사 시맨틱 검색 구현

**기술 스택**: `Node.js` `Express` `FastAPI` `React` `MySQL` `Firebase` `OpenAI API` `LangChain` `Selenium` `FAISS`

---


### 핵심 역량

**Backend**
- Spring Boot, JPA/QueryDSL, Spring Security, JWT 인증
- Solidity (ERC-721), Web3j, Ethereum 스마트 컨트랙트 설계 및 연동
- IPFS (Pinata), OAuth 2.0 소셜 로그인
- Redis 캐싱, Kafka 메시지 큐

**Frontend**
- React, Zustand 상태 관리
- WebRTC (LiveKit), 무한 스크롤
- 반응형 디자인, Protected Routes
