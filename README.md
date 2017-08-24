# JSP Ajax 회원가입 기능구현 강좌

ref. https://www.youtube.com/watch?v=XxeLEMC5jzA&list=PLRx0vPvlEmdCJ1TvP12_ACTV_9SvKw9TI

## 1강 - 프로젝트 소개 및 회원가입 화면 디자인

- Dynamic web project 생성
- bootstrap 적용(ver 3.3.7) 압축 풀고 프로젝트폴더/WebContent 에 복사
- index.jsp 추가 - language="java" 제거 charset,encoding "UTF-8" 변경
- 회원가입 폼 html 작성 custom.css 작성 font 설정
- - -

## 2강 - 데이터베이스 구축 및 연동

- mysql 연동 UserDAO.java UserDTO.java 생성
- jdbc 설치 후  WEB-INF lib에 추가 
- db my.ini 추가, shcema.sql 추가 
- mysql Connector 설치 WEB-INF/lib 폴더 밑에 jar 파일 복사
- - -

## 3강 - 회원가입 기능 구현하기

- servlet 생성 UserRegisterServlet (Web.xml 수정)
- UserRegisterServlet에 맞게 userDAO 수정
  - DB와 JSP 연동시에 디비 접근해서 쿼리문을 수행하는 기능을 하는 클래스
- Tomcat console로 DB 성공 했는지 확인 어려움으로 mysql 실행해서 직접 테이블 확인하는것이 좋음
 - - -
 
## 4강 - 사용자 친화적인 메시지 알림창 구현하기 

- index.jsp 수정 <%%> ejs 문법 사용 modal 팝업 이용
- servlet을 통해서 messageContent messageType이 결정됨
 - - -
 
## 5강 - 회원가입 중복 체크 및 프로젝트 완료

- @WebServlet("") 입력후 create annotation 해야 함 오른쪽 마우스 누른후 2번째 더블클릭
- 비밀번호 확인 onkeyup 사용 해서 함수 호출
- class name panel-warning은 background 빨강색 or 노란색, panel-success 는 초록색이다.
 