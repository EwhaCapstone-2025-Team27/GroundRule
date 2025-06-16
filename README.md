# 성큼성큼
청소년이 성에 대해 건강하고 자연스럽게 배울 수 있도록 돕는 AI 기반 성교육 서비스입니다.

##  프로젝트 개요
성큼성큼은 청소년들이 신뢰할 수 있는 성교육 정보를 AI 챗봇을 통해 자유롭게 질문하고 대답받을 수 있는 플랫폼입니다.
기존의 교과 위주의 성교육이 놓치기 쉬운 실생활 고민, 민감한 주제에 대해 친구처럼 편하게 이야기할 수 있도록 설계했습니다.

##  주요 기능
- ChatGPT 기반 AI 챗봇: 자유로운 질문에 대한 응답 제공
- 성 지식 수준 진단 테스트
- 관심 키워드 기반 콘텐츠 추천

##  사용 기술
- **Frontend**: React.js
- **Backend**: Spring Boot (Java)
- **Database**: MySQL
- **AI API**: OpenAI GPT-3.5-turbo
- **Vector DB**: FAISS (Facebook AI Similarity Search)

##  프로젝트 구조
```
/backend
├── src/main/java/com/seongkeumkeum
│ ├── controller # REST API Controller
│ ├── service # 비즈니스 로직
│ ├── model # Entity, DTO 등
│ └── repository # JPA 리포지토리
/frontend
├── src/components # React 컴포넌트
├── src/pages # 페이지 구성
└── src/services # API 통신
```
