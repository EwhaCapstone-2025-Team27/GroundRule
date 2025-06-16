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
seongkeumkeum-project/
│
├── /backend                     # Spring Boot 기반 백엔드
│   ├── controller               # REST API 엔드포인트 정의
│   ├── service                  # AI 호출 / 벡터 검색 / DB 접근 등 비즈니스 로직
│   ├── model                    # Entity, DTO 클래스 정의
│   └── repository               # JPA Repository (MySQL DB 연동)
│
├── /frontend                    # React 기반 프론트엔드
│   ├── components               # UI 컴포넌트 (ChatBox, Profile 설정 등)
│   ├── pages                    # 질문 페이지, 테스트 페이지 등 각 화면 구성
│   └── services                 # API 요청 정의 파일 (axios 등)
│
├── /ai_pipeline                 # Python 기반 AI 파이프라인 (Colab / 서버)
│   ├── ocr_processing.py        # 성교육 PDF → 텍스트 추출 (pytesseract, pdf2image)
│   ├── text_cleaning.py         # 정규표현식 기반 텍스트 정제 스크립트
│   ├── embed_and_index.py       # OpenAI 임베딩 + FAISS 저장
│   ├── query_and_rephrase.py    # LangChain RAG + GPT 응답 + 말투 후처리
│   └── vector_store/            # 저장된 FAISS index, .pkl 파일들
│
└── /docs                        # 보고서, 기술 설명서, 실험 결과 등 문서 모음
```
