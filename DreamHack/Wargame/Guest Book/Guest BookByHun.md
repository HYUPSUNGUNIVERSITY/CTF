# 풀이 아직 못함

5/30

게스트북이라는 게시판에 하이퍼링크를 걸고 클릭하면 cookie가 출력되게 만듬

실제로 cookie가 확인되는 것을 보고 아이디어가 생각남

클릭하면 자신의 cookie가 출력되는 게시글을 쓰고 관리자에게 report를 하면 admin의 쿠키를 알 수 있겠구나

<br>

-> 문제 정작 내 화면에는 good이라는 문자열만 보임

-> 해결방안(아직 못해봄) window.postmessage를 이용해서 parent화면에 message출력하게 하면 내 화면에 관리자의 쿠키가 나올 수 있겠구나

지금까지 작성된 payload a는 쿠키 출력 b는 postmessage를 이용(미완...)

[a](javascript:/alert/.source+[URL+[]][0][12]+/document.cookie/.source+[URL+[]][0][13] instanceof{[Symbol.hasInstance]:eval};)

[b](javascript:/parent.postMessage/.source+[URL+[]][0][12]+/document.cookie/.source+[URL+[]][0][13] instanceof{[Symbol.hasInstance]:eval};)


<br>
P.S.

관리자에게 게시글을 report하면 하이퍼링크가 클릭될거라 강하게 믿고있음🙏🙏🙏근거없는 뇌피셜 (._. )
