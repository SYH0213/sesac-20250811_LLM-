
# LLM과 API의 개념 및 관계

## 1. LLM (대규모 언어 모델)
- **정의**  
  - **Large Language Model**: 대규모 텍스트 데이터를 학습해 언어를 이해·생성하는 AI 모델.
- **주요 특징**
  1. **문맥 이해**: 이전 단어를 기반으로 다음 단어 예측
  2. **다양한 작업 수행**: 번역, 요약, 코드 작성, 질의응답 등
  3. **범용성**: 구조 변경 없이 다양한 주제 처리 가능
- **예시**  
  - OpenAI GPT 시리즈, Anthropic Claude, Google Gemini, Meta LLaMA, Mistral 등

---

## 2. API (응용 프로그램 인터페이스)
- **정의**  
  - **Application Programming Interface**: 프로그램과 프로그램이 데이터를 주고받는 규칙과 방법.
- **주요 역할**
  1. **접근 방법 제공**: 내부 로직을 몰라도 기능 사용 가능
  2. **데이터 교환 표준화**: JSON, XML 등 규격 사용
  3. **보안·인증**: API 키, 토큰 등으로 접근 제어
- **예시**
  - REST API, GraphQL API, WebSocket API
  - 날씨 API, 지도 API, 결제 API

---

## 3. LLM과 API의 관계
- LLM은 그 자체로 거대한 모델이지만, 일반 사용자가 직접 접근하지 않고 **API 형태**로 제공됨.
- **흐름**
  1. LLM 제공자(OpenAI, Google 등)가 모델을 서버에 배포하고 API 엔드포인트 제공
  2. 개발자가 API 키로 인증 후 HTTP 요청(프롬프트 포함)을 전송
  3. 서버가 LLM에 요청 전달
  4. LLM이 추론(Inference) 수행 후 JSON 형태로 응답 반환
  5. 앱/웹 서비스에서 JSON 파싱 후 UI에 표시

---

## 📌 비유
- **LLM** = 거대한 "두뇌"
- **API** = 두뇌와 대화할 수 있는 "전화선" 또는 "통역기"

---

## 📊 간단 비교표

| 항목 | LLM | API |
|------|-----|-----|
| 정의 | 언어 이해·생성 AI 모델 | 프로그램 간 데이터 교환 인터페이스 |
| 역할 | 답변·생성·분석 수행 | LLM 접근 경로 제공 |
| 제공자 | OpenAI, Google, Meta 등 | API 서버 운영자 |
| 사용자 | API 서버를 통해 간접 사용 | LLM 호출, 데이터 처리 |
| 예시 | GPT-4, Claude 3, Gemini 2.5 | ChatGPT API, Gemini API |
