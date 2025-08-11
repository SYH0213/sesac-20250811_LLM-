
# LangChain, OpenAI API, Gemini API의 역할과 관계

## 1. LangChain
- LLM 기반 애플리케이션 개발 프레임워크.
- 문서 분석, 요약, 챗봇, RAG 등 다양한 기능을 모듈화하여 제공.
- OpenAI, Google Gemini 등 수많은 LLM 및 외부 도구와 통합 가능.

## 2. OpenAI API
- OpenAI LLM(GPT‑계열 등)에 접근할 수 있는 REST 혹은 라이브러리 기반의 엔드포인트.
- API 키를 통해 인증 후 요청/응답 처리.
- LangChain에서는 `langchain-openai` 모듈로 쉽게 연동 가능.

## 3. Gemini API
- Google DeepMind의 멀티모달 LLM 시리즈(Gemini)에 접근 가능한 API.
- OpenAI 라이브러리와 호환되며, REST 방식으로도 사용 가능.
- LangChain에서는 `langchain-google-genai` 등을 통해 편리하게 사용 가능.

## 관계 요약

| 구성 요소     | 역할 |
|--------------|------|
| LangChain     | LLM 애플리케이션 구축 프레임워크 |
| OpenAI API    | OpenAI 모델 호출 및 응답 처리 |
| Gemini API    | Google Gemini 모델 호출 및 응답 처리 |

**LangChain**은 이들 API를 추상화된 방식으로 연결해주는 모듈 역할을 하며,  
개발자는 원하는 LLM 제공자를 선택하여 보다 쉽게 애플리케이션을 구축할 수 있습니다.
