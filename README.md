## 📝도서 대출 서비스 만들기
내가 원하는 책이 근처 도서관에 있는 지 찾아볼 수 있도록 도와주는 서비스 입니다.

## 스택 ⚙
* Spting Boot 3.2.1
* Spring Data JPA
* MySql Driver
* Thymeleaf
* OAuth2 Client
* Spring Security
* JWT

## 파트 분배 🙋
팀원 - 5명 <br>
로그인 API - 1명 <br>
프론트 관리 - 1명 <br>
공지사항 - 1명 <br>
Q&A - 1명 <br>
도서 API - 1명 <br>

## 담당한 기능 💻
* 로그인 기능 
* 검색 기능

## 담당한 기능 보기 👀
[여기를 눌러 주세요](https://github.com/mad-cost/Likelion_team6/blob/main/md/sixsenses.md "Click")

## 회고 🤔
프로젝트를 시작 할 때, 자진해서 OAuth2를 하겠다고 팀원들에게 말하였습니다. 왜냐하면 다른 파트에 비해서 나 자신에게 가장 큰 공부가 될 것 같았기 때문입니다.
<br>
- 협업<br>
팀원이 구현하지 못한, 검색 기능을 대신 구현해 줬습니다. 처음 접하는 새로운 기능을 완성했을 때 느끼는 만족감이 나를 한 층 더 성장하는 개발자로 만들어  주는 것 같습니다.

- 트러블 슈팅<br>
JWT 로그인 방식에 대한 이해가 부족하여 Token 방식과 Session 방식을 혼합하여 사용하는 실수를 범하였습니다. <br>
Token을 사용하기 위해 Stateless를 설정하였지만, 모든 페이지에 대하여 세션 기반 인증 방식인  `.hasRole()`을 적용하여 권한을 부여하였습니다.

- 해결 과정 <br> 
멘토님이 Token 방식과, Session 방식의 차이점에 대해서 찾아보라고 조언을 해주셨고, Token 방식에서 Stateless를 설정하는 이유와 .csrf( )를 disable로 주는 이유를 이해하면서 문제를 해결하였습니다.
