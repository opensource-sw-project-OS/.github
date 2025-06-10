
# 📊 소비와 감정을 함께 기록하는 Project OS

**사용자의 지출 기록과 감정 기록을 통합 관리하여, 감정 인식 기반의 소비 관리 및 정신 건강 증진을 돕는 웹 애플리케이션입니다.**

<br>

---

## 💻 주요 목표

💡 **하루 동안의 소비 내역과 기분을 입력**  
사용자는 하루 단위로 지출 내역과 감정을 기록

💡 **소비 패턴과 감정 변화를 시각화된 차트로 확인**  
기록된 데이터를 기반으로 소비 성향과 감정 흐름을 시각적으로 한눈에 확인

💡 **감정 기록을 통한 스트레스 인식과 정신 건강 관리**  
일상 속 감정 변화를 기록함으로써 스스로 감정 상태를 인식하고, 정신 건강을 돌볼 수 있는 기회를 제공

<br>

---
## 📜 GitHub 규칙
#### 커밋 메시지 규칙
- feat: 새로운 기능 추가
- fix: 버그 수정
- docs: 문서 수정 (README.md)
- style: 포맷 변경, 세미콜론 누락 등 (코드 변경 없음)
- refactor: 코드 리팩토링
- test: 테스트 코드 추가/수정
- chore: 빌드 업무 수정, 패키지 매니저 설정 등
- delete: 파일 삭제

#### 커밋 규칙
팀원 개별 repository에 fork 후 PR

#### PR (Pull Request) 규칙
- 제목: [태그] 간단한 작업 요약
- 본문: 작업 내용 / [기타 참고 사항]

<br>

---

## 📎 차별점 : 많은 오픈소스 사용
🔖 **Three.js** 감정 캐릭터를 3D로 시각화하기 위한 WebGL 라이브러리 - 따로 glb 파일 다운받아 해당 오픈소스로 3D 캐릭터 표시

🔖 **GLTFLoader / OrbitControls** Three.js에서 제공하는 3D 모델 로딩 및 카메라 컨트롤 기능

🔖 **Chart.js** 지출 데이터를 시각화하기 위한 차트 라이브러리

🔖 **affirmations** 사용자에게 긍정 문구 출력

🔖 **Cropper.js** 이미지 업로드 후 크롭 기능

🔖 **Korean_sentiment_analysis** 한국어 감정 분석용 딥러닝 모델. 감정을 자동으로 분류하는 기능

🔖 **FullCalendar** 웹 페이지에 달력(캘린더) UI를 쉽게 구현 - 일정 추가, 드래그 이동, 일간/주간/월간 뷰 전환 등

🔖 **Tesseract** OCR(광학 문자 인식) 기능을 제공

<br>

---

## 주요 기능
### 🔐 회원 관리
- **회원가입/로그인 기능** (bcrypt 해싱, JWT 기반 인증)
- JWT 토큰을 활용한 API 접근 권한 제어

<br>

### 🧾 지출 및 감정 입력
- **OCR 기반 영수증 인식** (Crop → 이미지 처리 → 텍스트 추출)
- 사용자의 감정 입력 및 분석 결과 저장
- 감정에 따른 문장 분석 및 원인 추론 기능
  ![image](https://github.com/user-attachments/assets/d25927e9-b799-4981-9583-1898e1174c34)


<br>


### 📊 지출 시각화 대시보드
- 감정별 지출 총액 그래프
    - 최근 30일간의 지출 중 가장 많았던 감정을 출력
    - 각 감정별로 지출의 몇%를 차지하는지 확인
    - 지출을 많이하는 감정에 유의하도록 하는 기능
  ![image](https://github.com/user-attachments/assets/fee19dc5-3260-464d-8d3a-234bfe82371d)

<br>


- 일별 감정 및 지출 변화 추이
    - 최근 30일간의 일별 지출 시각화
    - 감정 함께 확인 가능
  ![image](https://github.com/user-attachments/assets/d154327a-dba6-4ad8-80fc-edb0384b205a)

<br>


- 감정 변화 라인차트 (내 감정 확인)
    - 최근 30일간의 일별 감정 시각화
  ![image](https://github.com/user-attachments/assets/e7067af0-8258-484b-b60a-bc4964a892e9)

<br>


- 카테고리별 지출 분석
  - 최근 30일간의 일별 감정 시각화
  - 사용자가 어떤 카테고리에서 지출을 많이하는지 확인
  ![image](https://github.com/user-attachments/assets/762ddbb2-f97f-485e-952b-09fbfb029d5e)

<br>


- 이번 달 예산 대비 남은 금액 시각화 (도넛 차트)
    - 이번달 예산 입력시 남은금액 / 초과금액 시각화
  ![image](https://github.com/user-attachments/assets/1e140fbc-c88b-4872-9561-44a65abf566f)

<br>


- 달력 기반 감정 + 지출 통합 보기
    - 사용자가 지금까지 입력한 모든 지출과 감정을 한눈에 확인 가능!
  ![image](https://github.com/user-attachments/assets/d4a17ab3-467c-4f05-8c2c-157dbd580b7a)

<br>


- 주간 감정 요약 및 긍정 문구 제공 (다이어리 탭)
    - 사용자의 감정 기록 확인
    - 이번주의 평균 감정 시각화
  ![image](https://github.com/user-attachments/assets/17ec72e1-ce37-4a2a-bdc6-62eafb5a4ffb)

<br>


## 🤖 감정 분석 로직

- 감정 분류: `nlp04/korean_sentiment_analysis_dataset3_best` 모델 사용
- 원인 추출: `은전한닢 (Mecab)` 형태소 분석기를 통해 규칙 기반 파싱
- 분석된 감정 및 원인을 기반으로 **템플릿 문장 생성**
- 부정 감정 시 공감 문구를 출력하여 사용자 위로


---

### MySQL 데이터베이스
![image](https://github.com/user-attachments/assets/7c665c50-586b-4e23-9927-2e95758cb464)

```SQL
-- 데이터베이스가 없다면 생성, 명시한 DB 사용
CREATE DATABASE IF NOT EXISTS receipt_app;
USE receipt_app;

-- user 테이블 생성 (변동 없음)
CREATE TABLE IF NOT EXISTS user (
    user_id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50) NOT NULL,
    password VARCHAR(255) NOT NULL
);

-- receipt 테이블 생성 (자료형 변경 반영)
CREATE TABLE IF NOT EXISTS receipt (
    receipt_id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
    user_id INT NOT NULL,
    receipt_date DATE NOT NULL,
    category VARCHAR(50) NOT NULL,
    total_amount INT NOT NULL, -- DECIMAL에서 INT로 다시 변경
    emotion_type VARCHAR(20) NULL COMMENT '영수증에 기록된 감정 유형',
    emotion_description TEXT NULL COMMENT '감정에 대한 설명',
    FOREIGN KEY (user_id) REFERENCES user(user_id) ON DELETE CASCADE
);
```

---

## 📝 Project Log
### 🌟백엔드 및 프론트엔드의 상세 구현 내용 및 수정 사항은 각 레포지토리의 README에 정리되어 있습니다.🌟

<br>

### 2025-04-30
- 회의 내용
  - sentiment.js는 한국어 인식불가. 한글지원 오픈소스 KNU 감성 사전으로 변경
  - 감정 표시 -> 이모티콘 사용

- 다음 회의 내용
  - 백엔드와 프론트엔드간 주고받는 데이터 형식, 형태 논의
 
<br>

### 2025-05-09
- 회의 내용
  - 깃허브 규칙 명문화
  - 영수증 OCR 인식 : 기존 Tesseract.js에서 변경 -> OpenCV 시도 예정
  - 지도 식당 가격 api 문제 -> 학교 주변 식당 한정 크롤링
  - 감정분석 js 시도 예정
  - db 및 api 명세서 일정 논의
  - 다음 발표 내용 논의
 

<br>

### 2025-05-16
- 회의 내용
  - 구체적인 프론트엔드-백엔드 통신 논의
    - 사용자가 감정 상세 설명 텍스트 입력 시, 백엔드로 넘어가서 이를 분석하여 감정을 판정한 뒤 결과값을 프론트엔드에 보내주고, DB에도 저장
    - 사용자가 영수증 이미지를 넣으면, 백엔드에서 OCR 인식 후 결과값을 프론트엔드에 보내주고, DB에도 저장
    - 사용자 회원가입 시 username, password 백엔드로 넘어가 DB에 저장
  - DB
    - User, Emotion 테이블 추가 
    - DB 구조 논의 및 테이블 명세서 작성
     ![image](https://github.com/user-attachments/assets/4c53f4c7-c2cf-471a-b790-6072de20f52d)
  - 다음 주 발표 추가 내용 논의

<br>

 ### 2025-05-19
- 회의 내용
  - DB 구조 수정 회의 진행 : 테이블 3개 형태
  - 영수증, 감정, 사용자 테이블 각각 저장
 

<br>

 ### 2025-05-23
- 회의 내용
  - 감정과 지출 출력 형태 논의
  - 감정 지출 입력 페이지, 그래프 등 UI변경
  - 테이블 재정의 : 영수증과 감정 테이블 통합
    ![image](https://github.com/user-attachments/assets/ab7b48f7-7a3b-44b5-ab67-fd83405778f1)

  - 기능 추가 논의
      - 감정별 그래프 수정
      - 달력 탭 추가


<br>

 ### 2025-05-28
- 회의 내용
  - db 테스트 방법 논의
  - 영수증 입력 및 감정 입력 형태 변경
  - 감정을 이용한 추가 기능 논의
  - API 연동 계획
  - 사용자 협업툴을 이용한 API연동 흐름 논의
    ![image](https://github.com/user-attachments/assets/39cad509-0a71-4c2e-a2fb-9f048779ae77)

 <br>

 ### 2025-05-30
- 회의 내용
  - 프론드엔드 백엔드 연동
  - 감정, 카테고리 분류
  - 감정 분석 알고리즘 논의
  - 최종 발표 내용 논의
    
