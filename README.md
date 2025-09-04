# ✍️ 공감 챗봇 일기
> Kotlin을 활용하여 제작한 안드로이드 일기 앱으로, GPT API를 연동하여 사용자의 일기에 감성적인 공감과 반응을 제공

## 📌 주요 기능
- GPT 기반 감정 분석: 사용자가 작성한 일기 내용을 GPT API로 전송하여 감정을 분석하고, 분석 결과에 맞는 따뜻한 공감의 메시지를 이모지와 함께 제공
- 일기 작성 및 조회: SQLite 데이터베이스에 저장된 모든 일기를 날짜별로 조회하거나 전체 목록으로 확인할 수 있음
- 주간 감정 캘린더: 홈 화면에서 한 주간의 감정 이모지를 한눈에 파악
- 히스토리: 작성된 모든 일기를 리스트 형태로 모아볼 수 있음
- 사용자 설정:
  - 푸시 알림: 원하는 시간에 일기 작성을 잊지 않도록 알림 설정
  - 계정 관리: 사용자 이름과 챗봇의 이름을 자유롭게 변경
  - UI 커스텀: 앱 내의 글씨 크기를 조절하거나, 한국어/영어로 언어를 변경

## 🧩 작동 방식
1. 사용자는 회원가입 후 로그인하여 앱을 시작한다.
2. 일기를 작성하면 내용은 GPT API로 비동기 전송된다.
3. GPT는 내용을 분석하여 공감 응답과 감정 이모지를 생성한다.
4. 작성된 일기, 챗봇의 응답, 감정 이모지는 내부 SQLite DB에 날짜와 함께 저장된다.
5. 사용자는 홈 화면의 캘린더나 히스토리 탭에서 과거의 일기를 다시 열람할 수 있다.

## 🎨 스크린샷
1. **회원가입:** 회원가입 화면
<img width="625" height="1278" alt="signup" src="https://github.com/user-attachments/assets/08ad22a2-e70b-42c2-a959-aacc2ad8ec47" />
- 회원가입 성공
<img width="625" height="1278" alt="signup_finish" src="https://github.com/user-attachments/assets/41ad0d49-c54e-4dca-be68-7894050aa8e4" />

2. **로그인:** 로그인 화면
<img width="625" height="1278" alt="login" src="https://github.com/user-attachments/assets/7dd4b441-6cd6-4469-bc1e-530aa7c2ef0c" />

3. **홈 화면:** 주간 감정 캘린더와 날짜별 일기 조회가 가능한 메인 화면
<img width="625" height="1278" alt="success_login" src="https://github.com/user-attachments/assets/22490401-fc90-4c32-8efb-274d2b1dd921" />

4. **일기 작성:**
<img width="625" height="1278" alt="write_diary" src="https://github.com/user-attachments/assets/3c2853df-109e-485c-9b51-40e250b1fdcb" />

5. **일기 저장:**
<img width="625" height="1278" alt="save_diary kt" src="https://github.com/user-attachments/assets/73d8d45f-bf9f-48c9-bffc-16e1740aca0b" />

6. **일기 상세 페이지:**
<img width="625" height="1278" alt="view_diary" src="https://github.com/user-attachments/assets/962530bb-b066-4653-83f2-83420cab1e0d" />

7. **이모지 적용:**
<img width="625" height="1278" alt="show_emoticon" src="https://github.com/user-attachments/assets/1e19d434-a908-4132-8162-7cab85fdb7b2" />

8. **날짜 선택:**
<img width="625" height="1278" alt="select_date" src="https://github.com/user-attachments/assets/cb5f4991-2124-46c8-ad13-b7f0e08ac552" />

9. **히스토리 탭:**
<img width="625" height="1278" alt="history" src="https://github.com/user-attachments/assets/b1c5be19-35a7-4497-9676-c22ba465dbf1" />

10. **설정 탭:**
<img width="625" height="1278" alt="setting" src="https://github.com/user-attachments/assets/40898b30-be28-47cb-9633-4d34a0d2ad0d" />
- **계정**
<img width="625" height="1278" alt="account" src="https://github.com/user-attachments/assets/e499efe0-d472-4031-8505-7ea84d07bb8d" />
  - **이름 변경**
    <img width="625" height="1278" alt="change_name" src="https://github.com/user-attachments/assets/9d98d1ec-34a3-4a30-b769-df9e83e1d504" />

- **푸시 알림**
<img width="625" height="1278" alt="select_noti" src="https://github.com/user-attachments/assets/0b3822a8-8f18-47fd-babb-777cb2ce4993" />
  - **알림**
  <img width="625" height="1278" alt="noti" src="https://github.com/user-attachments/assets/e1ef4b72-1099-4fe8-bbb3-3c9b4ce5d1ec" />

- **글씨 크기**
  <img width="625" height="1278" alt="select_textSize" src="https://github.com/user-attachments/assets/86e6d9c6-b08f-41ba-a21a-0d5f7f43b184" />
    -**글씨 크기 변경**
    <img width="625" height="1278" alt="change_textSize" src="https://github.com/user-attachments/assets/1701c9db-3c9b-4afa-92c6-6a9f1d96de86" />

- **언어**
  <img width="625" height="1278" alt="select_lang" src="https://github.com/user-attachments/assets/9483f552-c59e-4aa7-8809-ded7c0ff98fd" />
  -**언어 변경**
  <img width="625" height="1278" alt="change_lang" src="https://github.com/user-attachments/assets/5fd75a36-cbe0-4d96-ac92-c6968ad5eb5f" />

-**로그아웃**
<img width="625" height="1278" alt="logout" src="https://github.com/user-attachments/assets/51e30ef8-87f6-4bb3-b394-4dcb410f44b0" />

## 🛠️ 주요 기술 스택
 - **Language:** Kotlin
 - **API & Networking:** Retrofit2, OkHttp, Gson (GPT API 연동)
 - **Asynchronous:** Coroutines
 - **Database:** SQLite
 - **Architecture & UI:** Android Jetpack (Fragment, LiveData), XML
 - **External API:** OpenAI GPT API

## 🧠 배운 점
- Retrofit과 Coroutine을 활용하여 외부 API(GPT)와 안정적으로 비동기 통신을 처리하는 방법을 익혔다.
- SQLite를 사용하여 사용자의 데이터를 앱 내부에 저장, 조회, 수정하는 로컬 데이터베이스 관리 능력을 길렀다.
- Fragment를 활용한 탭 기반 UI를 구현하고, 각 Fragment의 생명주기를 효과적으로 관리하는 방법을 학습했다.
- BroadcastReceiver와 NotificationManager를 이용해 앱이 꺼진 상태에서도 특정 시간에 푸시 알림을 보내는 기능을 구현했다.
- 다국어 지원, 글씨 크기 동적 변경 등 사용자 경험(UX)를 고려한 개인화 기능을 설계하고 개발하는 경험을 쌓았다.

## ✅ 향후 개선점
- Firebase와 같은 클라우드 데이터베이스를 도입하여 여러 기기에서 일기 데이터 동기화 기능 추가
- 단순 이모지 표기를 넘어 일기 내용에 기반한 긍정/부정 수치 등 다각적인 감정 분석 통계 기능 제공
- Jetpack Compose를 학습하여 기본 XML 레이아웃을 리팩토링하고, 선언형 UI 개발 방식 도입
- JUnit, Espresso 등을 활용하여 코드 안정성 확보를 위한 유닛 테스트 및 UI 테스트 코드 작성
