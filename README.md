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

## 내가 만든 기능 💻
* 로그인 기능 
* 검색 기능

## 내가 만든 기능 간략히 보기 👀
[여기를 눌러 주세요](https://github.com/mad-cost/Likelion_team6/blob/main/md/sixsenses.md "Click")

## 회고 🤔
첫 팀 프로젝트를 하면서 가장 고민했던 점은 '역할 분담과 협업' 이었던 것 같다. <br>
- 역할 <br>
파트를 분배함에 있어, 기능을 중심으로 나눌지, 페이지를 중심으로 나눌지, 혹은 구현이 어려운 순서부터 차근차근 해결해 나아갈지 갈피를 잡지 못했던 것 같다. <br>
- 협업 <br>
깃 브랜치를 처음 사용하다 보니 시간을 많이 잡아먹었고, 충돌이 일어날 때마다 당황을 했었지만, 결국엔 하면 할수록 익숙해지는게 깃(Git)인거 같다. <br>
팀원이 구현하지 못한, 검색 기능을 대신 구현해 줬는데 새로운 기능을 완성했을 때 느끼는 만족감이 나를 성장하는 개발자로 만들어 주는 것 같다. <br>
- 에러<br>
프로젝트를 시작 할 때, 자진해서 OAuth2를 하겠다고 팀원들에게 말하였다. 왜나하면 다른 파트에 비해서 나 자신에게 가장 큰 공부가 될 것 같았기 때문이다.
막상 프로젝트를 시작하니 크나큰 실수를 범하게 되는데 Stateless에 대한 이해가 부족하여 Session 방식과 Token 방식을 혼합하여 사용하는 실수를 범하였다. <br>
- 공부 <br>
Stateless = 클라이언트의 요청을 서버에서 상태를 기록하지 않는 접속 방식이다, `독립적`이다.<br>
즉, 로그인 후 다시 웹페이지에 접근하면 로그인 상태가 유지되지 않는다.
```java
Stateless, 
.sessionManagement(session -> session
                    .sessionCreationPolicy(SessionCreationPolicy.STATELESS)
            )
```

