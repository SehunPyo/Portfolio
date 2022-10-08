# Portfolio

### 🌑 프로젝트 목적

그동안 공부한 내용을 바탕으로 웹사이트를 제작하며 부족한 부분을 보완하고 역할을 수행할 수 있는 웹개발자로 성장하기.
##

### 🌒 프로젝트 개요

웹소설 작가를 꿈꾸는 작가 지망생이 무료로 작품을 연재하며 경험을 쌓고, 양질의 컨텐츠를 원하는 독자들이 무료로 작품을 즐기고 댓글을 통해 피드백을 주고받을 수 있는 웹소설 연재 플랫폼.
##

### 🌓 프로젝트 설명

● 시스템 구상도

![화면 캡처 2022-10-08 201233](https://user-images.githubusercontent.com/105040121/194704613-cffcc7c5-2a85-49af-b48c-1564de1e6672.png)

1. 클라이언트가 게시글 및 댓글 작성
2. Middleware를 통해 Database에 데이터 전달
3. Database에 저장 된 데이터를 클라이언트가 원하는 정보만 출력

● 주요 기능

1. 회원 가입 후 게시글 작성
2. 게시글 수정 및 삭제
3. 게시글 추천
4. 댓글 작성 및 삭제
5. 실시간 작품 랭킹
##

### 🌔 프로젝트 상세 설명

웹사이트 회원가입 당시 입력한 정보가 DB에 저장, 클라이언트가 로그인을 시도할 때 입력한 정보가 DB에 존재하면 로그인에 성공한 화면 송출, DB에 존재하지 않으면 로그인에 실패했다는 alert 메세지와 함께 로그인 창으로 이동한다.

클라이언트가 회원가입 당시 입력하는 정보를 바탕으로 DB를 조회해 중복확인 기능을 설계해 같은 아이디와 닉네임으로는 가입할 수 없게 제작한다.

로그인을 한 사용자는 게시글 작성 및 댓글 작성을 할 수 있고 게시글과 댓글 역시 DB에 저장된다. 로그인 정보는 Session에 저장되어 브라우저를 종료하지 않으면 사이트를 이동해도 로그인이 유지되게 설계하고, 세션에 저장되어 있는 로그인 정보 중 ID와 화면에 송출되고 있는 게시글 및 댓글의 ID가 일치하면 게시글을 수정 및 삭제할 수 있는 화면을 보여준다.

웹사이트를 제작 후 AWS(아마존 웹서비스)를 통해 서버를 배포하고 도메인 등록을 구현해보겠다.
##

### 🌕 개발 환경 구성

Back-End : Java11, JSP, Spring Boot 2.7.2, AWS

DB : MySQL

front : HTML5, CSS3, JavaScript

IDE : Visual Studio Code, Intelli J

라이브러리 : Lombok, Mybatis, Spring Security
##

### 🌠 웹사이트 디자인 구상

[ 메인화면 로그인 전 ]

<img src="https://user-images.githubusercontent.com/105040121/194705364-756fcb3b-60f1-4dd7-96a1-399c08099519.png" width="800" height="470"/>

[ 메인화면 로그인 후 ]

<img src="https://user-images.githubusercontent.com/105040121/194705543-38903df8-9d01-475e-9439-013d15097ff0.png" width="800" height="470"/>

[ 회원가입 ]

<img src="https://user-images.githubusercontent.com/105040121/194705576-41f61486-a45d-4d75-9c46-eb73caa1cc6d.png" width="800" height="470"/>

[ 카테고리 선택 후 ]

<img src="https://user-images.githubusercontent.com/105040121/194705619-8bad244b-ec31-4606-a999-133b8184925f.png" width="800" height="470"/>

[ 게시글 작성 ]

<img src="https://user-images.githubusercontent.com/105040121/194705648-72decbd7-0643-4764-a19a-c5761c3d5e7b.png" width="800" height="470"/>

[ 본인 게시글 확인 ]

<img src="https://user-images.githubusercontent.com/105040121/194705672-7ab8272f-9102-4477-872a-6970b74ab628.png" width="800" height="470"/>

[ 일반 유저 화면 ]

<img src="https://user-images.githubusercontent.com/105040121/194705745-82109b1f-52fd-4c8f-a9d1-573ca55fc686.png" width="800" height="470"/>

[ 댓글 작성 ]

<img src="https://user-images.githubusercontent.com/105040121/194705771-24218f8a-e275-4725-897b-f38144e018b5.png" width="800" height="470"/>
