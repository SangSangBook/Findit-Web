# FindIt - 이미지/비디오 텍스트 검색 및 계약서 분석 도구

FindIt은 이미지와 비디오에서 텍스트를 검색하고, YouTube 영상을 처리하며, 계약서를 자동으로 분석할 수 있는 강력한 도구입니다.

## 주요 기능

### 1. 이미지 텍스트 검색
- 이미지에서 텍스트 추출 및 검색
- 일반 검색 및 스마트 검색 모드 지원
- 검색된 텍스트에 동그라미로 하이라이트 표시
- 다중 텍스트 매칭 지원

### 2. 비디오 텍스트 검색
- 비디오 파일에서 텍스트 추출 및 검색
- 타임라인 기반 검색 결과 표시
- 검색된 텍스트의 시간대 자동 이동 기능
- 프레임 단위 텍스트 인식

### 3. YouTube 영상 처리
- YouTube URL을 통한 영상 처리
- 자동 다운로드 및 텍스트 추출
- 타임라인 기반 검색 결과 제공
- 영상 재생 및 시간 이동 기능

### 4. 계약서 분석
- 계약서 이미지 업로드 및 분석
- 주요 내용 자동 요약
- 계약 당사자, 주요 내용, 중요 날짜, 특이사항 추출
- 구조화된 요약 결과 제공

## 기술 스택

- Frontend: React, TypeScript
- Backend: Python, Flask
- OCR: EasyOCR, PaddleOCR, Tesseract, Google Vision
- AI: OpenAI GPT

## 설치 및 실행 방법

1. 저장소 클론
```bash
git clone [repository-url]
cd FindIt
```

2. 필요한 패키지 설치
```bash
# 백엔드 의존성 설치
pip install -r requirements.txt

# 프론트엔드 의존성 설치
npm install
```

3. 환경 변수 설정
`.env` 파일을 생성하고 다음 변수들을 설정:
```
OPENAI_API_KEY=your_openai_api_key
GOOGLE_CLOUD_VISION_API_KEY=your_google_vision_api_key
```

4. 서버 실행
```bash
# 백엔드 서버 실행 (포트 5001)
python app.py

# 프론트엔드 개발 서버 실행 (포트 3000)
npm start
```

## 사용 방법

### 이미지 검색
1. "이미지 업로드" 버튼을 클릭하여 이미지 파일 선택
2. 검색어 입력
3. "검색" 또는 "스마트 검색" 버튼 클릭
4. 검색된 텍스트가 동그라미로 표시됨

### 비디오 검색
1. "동영상 업로드" 버튼을 클릭하여 비디오 파일 선택
2. 검색어 입력
3. 검색 버튼 클릭
4. 타임라인에서 검색된 텍스트 확인 및 클릭하여 해당 시간으로 이동

### YouTube 영상 처리
1. YouTube URL 입력
2. "처리하기" 버튼 클릭
3. 영상 다운로드 및 처리 완료 후 타임라인 확인

### 계약서 분석
1. 계약서 이미지 업로드
2. "요약" 버튼 클릭
3. 자동으로 생성된 요약 내용 확인

## 주의사항

- 이미지 파일은 PNG, JPG, JPEG 형식 지원
- 비디오 파일은 MP4, AVI, MOV, MKV 형식 지원
- YouTube URL은 유효한 공개 영상 링크여야 함
- API 키는 반드시 유효한 키를 사용해야 함

## 라이선스

MIT License

## 기여

프로젝트에 기여하고 싶으시다면 Pull Request를 보내주세요.
