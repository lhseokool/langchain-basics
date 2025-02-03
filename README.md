# 한시간으로 끝내는 LangChain 기본기

인프런 강의 "한시간으로 끝내는 LangChain 기본기"를 위한 예제 코드 저장소입니다.

## 강의 소개

이 강의는 LangChain의 핵심 개념과 기본 기능을 1시간 안에 실습과 함께 배울 수 있도록 구성되어 있습니다.

## 학습 내용

### 1. LLM을 활용해서 답변을 생성하는 방법
- LangChain에서 다양한 LLM 서비스(Ollama, OpenAI, Azure OpenAI, Anthropic) 사용법
- API 키 설정 및 환경 변수 관리
- 기본적인 LLM 호출 방법

### 2. 랭체인 스타일로 프롬프트 작성하는 방법
- PromptTemplate 활용
- 변수가 포함된 템플릿 생성
- 메시지 기반 프롬프트 작성
- ChatPromptTemplate 활용

### 3. 답변의 형식을 컨트롤하는 방법
- 문자열 출력 파서(StrOutputParser) 사용
- Pydantic 모델을 활용한 구조화된 출력
- JSON 형식의 응답 처리
- 출력 형식 지정 및 파싱

### 4. LCEL을 활용한 랭체인 생성하는 방법
- LangChain Expression Language (LCEL) 소개
- 파이프 연산자를 활용한 체인 구성
- RunnablePassthrough를 활용한 복잡한 체인 구성
- 다단계 추론 체인 구현

### 5. 실전 응용 및 프롬프트 엔지니어링 팁
- Temperature 조절을 통한 일관성 확보
- 명확한 출력 형식 지정
- 시스템 메시지 활용
- 체인 연결을 통한 복잡한 작업 처리

## 필요 라이브러리

```bash
pip install langchain-ollama langchain-openai langchain-anthropic python-dotenv
```

## 실행 환경
- Python 3.11 이상
- Jupyter Notebook
- Ollama (로컬 LLM 실행용)

## 파일 구조
```
.
├── README.md
├── .env  # API 키 등 환경 변수 (생성 필요)
├── 2. LLM을 활용해서 답변을 생성하는 방법.ipynb
├── 3. 랭체인 스타일로 프롬프트 작성하는 방법.ipynb
├── 4. 답변의 형식을 컨트롤하는 방법.ipynb
├── 5. LCEL을 활용한 랭_체인_ 생성하는 방법.ipynb
└── 6. 지금까지 배운 내용 총정리 (feat. 프롬프트 꿀팁 살짝).ipynb
```

## 환경 변수 설정

- 필수아님
`.env` 파일을 생성하고 다음과 같이 API 키를 설정하세요:

```env
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
```

## 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다.
```
