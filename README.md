# Portfolio

### 목차

1. [프로젝트 목적](#-프로젝트-목적)
2. [프로젝트 개요](#-프로젝트-개요)
3. [프로젝트 설명](#-프로젝트-설명)
4. [프로젝트 상세 설명](#-프로젝트-상세-설명)
5. [개발 환경 구성](#-개발-환경-구성)
6. [웹사이트 디자인 구상](#-웹사이트-디자인-구상)
7. [개발 일지](#-개발-일지)
##

### 🌑 프로젝트 목적

그동안 공부한 내용을 바탕으로 웹사이트를 제작하며 동시에 부족한 부분을 공부해 보완하고 맡은 역할을 수행할 수 있는 웹개발자로 성장하기.
##

### 🌒 프로젝트 개요

웹소설 작가를 꿈꾸는 작가 지망생이 무료로 작품을 연재하며 경험을 쌓음과 동시에 자신의 작품을 세상에 알릴 수 있는 기회를 얻고, 양질의 컨텐츠를 원하는 독자들이 무료로 작품을 즐기고 댓글을 통해 피드백을 주고받을 수 있는 웹소설 연재 플랫폼.
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

***


### 🌠 개발 일지

### 2022. 10. 07

<img src="https://user-images.githubusercontent.com/105040121/194706210-e12e4a60-f5bd-4912-9e8a-64ad9072468f.png" width="800" height="470"/>

프로젝트 구상 및 디자인 시안 제작 후 VScode에서 HTML5와 CSS3로 웹 사이트 틀 제작.

<li>
  어려웠던 점 : 웹사이트의 구조를 이해하는 것에 어려움이 있었고, CSS를 이용해 자리 배치를 하는 것이 마음대로 되지 않아 힘이 들었다.
</li>
<li>
  해결 방법 : HTML과 컨테이너의 구조를 이해하고 Position과 Display, float 속성 등을 이용해 자리를 원하는 대로 배치하고 Margin 속성으로 세밀한 조정을 할 수 있었다.
</li>

##

### 2022. 10. 08

VScode에서 HTML5와 CSS3를 사용해 웹사이트 메인 화면 (로그인 전 화면) 제작, 회원가입 페이지 제작.

##

### 2022. 10. 09

<img src="https://user-images.githubusercontent.com/105040121/195035909-8d0cb3cc-0b40-4276-8193-52a652cf3dfe.png" width="800" height="470"/>

추천 수를 반영해 실시간 랭킹이 표시 될 작품을 네이버 카페 메인화면에 제작되는 방식으로 ul태그와 li태그, dl, dt, dd 태그를 이용해 구현했고, 오른쪽 div구역에 로그인 및 개인 정보를 확인할 수 있는 공간을 제작하기 시작했다.

<li>
  어려웠던 점 : ul태그와 li태그의 구조를 이해하는 것에 시간이 걸렸고 공간 배치가 가로로 정렬되는 것이 아니라 아래로 배치되어 처음 구상한 디자인과 차이가 많이 났다.
</li>
<li>
  해결 방법 : position을 absolut로 적용하고 사이즈를 조절, 양 옆 공간을 padding으로 넓히고 display를 inline으로 적용해 한 줄에 표현 될 수 있도록 했다.
</li>

##

### 2022. 10. 11

메인화면의 로그인&회원가입 영역 구현 및 카카오의 REST API로 카카오톡 로그인을 구현하기 위해 카카오 DEVEROPER에서 WEB에 들어가 API소스를 받고 적용하는 방법에 대해 찾기 시작했다.

##

### 2022. 10. 12

<img src="https://user-images.githubusercontent.com/105040121/195271517-98f679da-4276-4594-b133-5e9a8d9fb5fa.png" width="800" height="470"/>

<img src="https://user-images.githubusercontent.com/105040121/195271878-1cbafac8-6225-4270-bf02-ad8990c5d2fd.png" width="800" height="470"/>

api를 이용해 카카오톡 로그인을 구현하려고 카카오톡 API의 JavaScript소스를 가져와 구현하였다.

카카오톡 로그인 버튼을 클릭하면 카카오톡 로그인 화면으로 넘어가지만 아직 로그인이 실제로 되지는 않는다.
실제로 로그인이 되는가에 대한 부분은 추후에 Intelli J에서 JSP와 Spring Boot를 이용해 개발할 때 시도해보기로 한다.

##

### 2022. 10. 13

<img src="https://user-images.githubusercontent.com/105040121/195665609-7566f8bd-90c1-4a0f-aa8a-6d1b79222413.png" width="800" height="470"/>

메인화면 디자인 제작을 마무리하고 웹소캣을 활용한 실시간 채팅기능을 위한 디자인과 틀을 만들어 두었다.

<img src="https://user-images.githubusercontent.com/105040121/195665869-9bfd586b-eb6c-4b34-bb3d-1a144b547161.png" width="800" height="470"/>

회원가입 버튼을 클릭하면 회원가입(signin.html)으로 넘어가도록 설계하였고 정보를 입력하면 form태그를 활용해 method="get" 방식으로 회원가입란에 입력한 정보가 가입하기 버튼을 누르면 action에 입력된 사이트로 이동할 때 함께 넘어가게된다.

<img src="https://user-images.githubusercontent.com/105040121/195666289-e4fa8e3f-6af7-4de1-a0a0-2155fd77a8d3.png" width="800" height="100"/>

이처럼 입력한 정보가 url란에 표시되면 정보가 제대로 넘어온 것이다. get방식이 아닌 post방식으로 서버를 이동하면 정보는 넘어오되, url란에 입력한 정보가 나타나지 않는 것을 보니 개인정보나 민감한 정보를 넘길 때는 post방식으로 넘겨 보안을 하면 될 듯하다.

<li>
  어려웠던 점 : 단순히 input type=""을 이용하여 제작만 하면 되는 줄 알았는데 정보를 어떻게 넘길 것인가를 생각해보니 다른 방법이 필요한 듯 하였다.
</li>
<li>
  해결 방법 : form태그안에 input type="" 코드를 짠 뒤 name=""으로 이름을 지어주어야 정보가 제대로 넘어가고 그 정보를 넘길 방아쇠 역할로는 버튼이 아닌, input type="submit"을 사용해야 한다는 것을 알게되었다.
</li>
<li>
  궁금한 내용 : 14일부터는 기능 구현을 시작할텐데 form태그안에 코드를 짜고 submit을 이용해 사이트가 넘어갈 때 정보가 함께 넘어간다면, 그 것과 DB에 정보를 입력하기 위해 CRUD코드를 작성하는 것과는 다른 개념인가?
  
  쉽게 풀어서 말하자면, 사이트가 넘어갈 때 정보가 넘어가는 것은 정확히 어떤 상황에서 사용하는 것인가에 대한 부분을 아직 확실히 모르겠다. 사이트를 제작하며 동시에 공부를 함께 하고 있는데 일단 내 머리로 이해한 내용대로라면 백엔드 서버에 정보를 저장할 때 form태그를 사용한다는 것인데 CRUD와 함께 사용하는 것인지 각자 역할이 다른 것인지는 JSP와 Spring, Spring Boot 등을 사용해 기능 구현을 해보아야 감이 잡힐 듯 하다.
</li>
