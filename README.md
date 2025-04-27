# 텍스트 기반 JSON 생성기

## 1. 프로젝트 개요
- **제목**: 텍스트 기반 JSON 생성기
- **선택한 문제 유형**: 예시과제 3번 (자연어 처리 및 정보 추출)
- **목표**: OpenAI API를 활용하여 자연어 설명에서 구조화된 JSON 정보를 자동으로 추출하는 시스템을 구현합니다.

## 2. 시스템 구성
- **사용한 모델**: `gpt-4o-mini`
- **사용한 주요 파라미터**
  - `temperature`: 0.2
  - `max_tokens`: 300
- **라이브러리 및 환경**
  - Python 3.13
  - `openai` (OpenAI API 호출)
  - `dotenv` (환경 변수 로딩)
  - `json` (JSON 데이터 처리)

## 3. 실행 방법
1. `.env` 파일에 OpenAI API 키 저장
   ```
   OPENAI_API_KEY=your-api-key-here
   ```
2. 필요한 라이브러리 설치
   ```
   pip install openai python-dotenv
   ```
3. 메인 실행 파일 실행
   ```
   python main.py
   ```

## 4. 예시 입력 및 출력
- **입력 예시**:
  ```
  서울에 있는 삼성전자는 데이터 분석가를 목집 중이며, Python과 SQL이 필수입니다.
  ```
- **출력 예시**:
  ```json
  {
    "company": "삼성전자",
    "location": "서울",
    "position": "데이터 분석가",
    "skills": ["Python", "SQL"]
  }
  ```

## 5. 파일 구성
| 파일명 | 설명 |
|-----------|-------|
| `main.py` | 프로젝트 메인 실행 파일 |
| `.env` | open ai api key |
| `OpenAI API report.pdf` | 분석 보고서 |
| `README.md` | 실행 안내서 (본 문서) |

## 6. 참고자료
- 강의 자료 Chapter 1~3 (프롬프트 설계 및 API 호출)
- [how to convert a string to json](https://www.freecodecamp.org/news/python-json-how-to-convert-a-string-to-json/)
- [json 파싱하기](https://schatz37.tistory.com/64)

## 7. 기타
- 코드에는 적절한 주석(comment)이 포함되어 있습니다.
- 실패한 테스트 사례도 보고서에 기술되었습니다.
  
