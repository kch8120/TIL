<h1>HTTP</h1>
<h2>
<a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2F20131108_291%2Fcom7321_1383905922311X2Oho_JPEG%2F20131108_191555.jpg&type=sc960_832"><목차></a><hr>
- HTTP는 뭐고 어떤 역할을 할까?<br>
- HTTP는 어떤 구조일까?<br>
- HTTP Method가 뭘까?<br>
- HTTP 상태코드가 뭘까?<br>
- HTTP의 Header, Body가 뭘까?</h2>
<hr>
<h2>HTTP가 뭘까?<br><br></h2>
<h3>
HTTP는 웹에서 하이퍼텍스트,<br><br>
즉, 클라이언트와 서버간의 데이터를 주고받는 규칙이다.<br><br>
HTTP는 인터넷의 핵심이며, 사용자가 웹페이지, 이미지, 동영상 등 콘텐츠를 요청하고<br><br>
서버가 이를 응답하는 데 사용된다.
</h3>
<h4>
하이퍼텍스트가 뭘까?<br><br>
하이퍼텍스트는 하이퍼링크와 비슷한 개념이다.<br><br>
단지 하이퍼링크를 좀 더 고급지게 개조시킨 것이 하이퍼텍스트인 것이다.<br><br>
</h4>

<h2>HTTP는 어떤 구조일까?<br><br></h2>
<h3>HTTP는 기본적으로 클라이언트-서버 모델을 사용하는 요청-응답 기반 프로토콜이다.<br><br>
클라이언트가 뭔가를 요청하면, 서버가 응답하는 과정에서 사용되는 프로토콜이 HTTP인 것이다.<br><br><br>
예를 들어 웹사이트에 방문해서 영상을 보거나, 스마트폰으로 앱을 사용하거나,<br><br>
브라우저로 데이터를 업로드할 때 클라이언트는 서버에 HTTP 요청 메시지를 보낸다.<br><br><br>
그럼 HTML 파일, 이미지, 동영상 같은 콘텐츠 리소스를 제공하는 서버는<br><br>
클라이언트에 응답 메시지를 회신한다.<br><br>
또, HTTP에는 무상태성이라는 게 존재하는데,<br><br>
이는 각 요청과 응답은 독립적이며, 이전 요청의 상태를 기억하지 않는다는 걸 나타낸다.<br><br>
HTTP는 상태 유지를 위해 쿠키, 세션 등을 활용한다.<br><br>
</h3>
<h2>
HTTP Method가 뭘까?<br><br></h2>
<h3>
HTTP Method에는 GET, POST, PUT, PATCH가 있다.<br><br>
1. GET<br><br>
GET 메서드는 서버로부터 데이터를 가져오기 위해 사용된다.<br><br>
요청 데이터를 URL의 Query String 형태로 전달하며,<br><br>
주로 읽기 요청에 쓰인다.<br><br>
특징으로는<br><br>
요청 데이터가 URL에 노출된다.<br><br>
요청 데이터 크기 제한이 있다.<br><br>(브라우저마다 다르지만 일반적으로 약 2000자 정도이다.)<br><br>
캐싱(Caching)이 가능하다.<br><br>
멱등성을 가진다.<br><br>(동일한 요청을 여러 번 보내도 결과가 같다.)<br><br>
2. POST<br><br>
POST 메서드는 주로 서버에 데이터를 생성할 때 사용되며,<br><br>
요청 데이터를 요청 본문에 담아 전달한다.<br><br>
특징으로는<br><br>
요청 데이터가 URL에 노출되지 않아 보안상 GET보다 상대적으로 유리하다.<br><br>
데이터 크기 제한이 GET에 비해 상대적으로 적다.<br><br>
(서버 설정에 따라 다르나 일반적으로 크기가 더 크다.)<br><br>
캐싱이 기본적으로 불가능하다.<br><br>
멱등성을 보장하지 않는다.<br><br>(같은 요청 반복 시 매번 다른 결과가 나올 수 있다.)<br><br>
3. PUT<br><br>
PUT 메서드는 리소스 전체를 수정하거나, 존재하지 않을 경우 새롭게 생성할 때 사용된다.<br><br>
특징으로는<br><br>
리소스의 전체적인 교체를 수행한다.<br><br>
멱등성을 보장한다.(여러 번 요청해도 동일한 결과를 보장한다.)<br><br>
4. PATCH<br><br>
PATCH 메서드는 리소스의 부분적인 수정을 위해 사용된다.<br><br>
특징으로는<br><br>
리소스 일부 필드만 수정할 때 사용한다.<br><br>
요청 본문에 변경하고자 하는 부분 데이터만 포함된다.<br><br>
일반적으로 멱등성을 보장하지 않는다.<br><br>
</h3>
<h4>Query String이란<br><br>
"https://search.naver.com/search.naver?ssc=tab.image.all&mode=column&section=image&query=%EA%B0%90%EC%82%AC%ED%95%A9%EB%8B%88%EB%8B%A4%20%EC%A7%A4&res_fr=0&res_to=0&sm=tab_opt&color=&ccl=0&nso=so%3Ar%2Cp%3Aall&recent=0&gif=1&nso_open=0&pq=#imgId=image_sas%3Ablog_f9d6bb89c4a175b4abaa11a5fa2318ea"<br><br>
이 링크에서 search.naver'?' 다음에 나오는 모든 글자가 Query String이라고 생각하면 된다.</h4>
<h2>HTTP Status Code가 뭘까?</h2>
<h3>
200 = OK(요청이 성공했다.)<br><br>
404 = 찾을 수 없음(가장 대표적인 코드이다.<br><br>
서버가 원본 서버가 대상 리소스에 대한 최신 표현을 찾지 못했거나<br><br>
존재한다는 사실을 알리고 싶지 않은 경우이다.)<br><br>
500 = 내부 서버 오류(서버가 요청을 처리할 수 없게 만드는<br><br>
예기치 않은 상황을 만났음을 나타낸다.)<br><br>
</h3>
<h2>HTTP의 Header Body가 뭘까</h2><br><br>
<h3>HTTP의 Header는 클라이언트와 서버가 요청 또는 응답으로<br><br>
부가적인 정보를 전송할 수 있도록 한다.<br><br>
또, Header는 대소문자를 구분하지 않는 이름과 콜론 다음에 오는 값으로 이루어져있다.<br><br>
Body는 해당 요청에 대한 실제 메시지/내용을 전송한다.<br><br>
Header는 일반 Header, 요청 Header, 응답 Header로 나뉜다.<br><br>
일반 Header는 요청/응답이 생성된 날짜 및 시간과 같은<br><br>
HTTP 통신에 대한 일반적인 정보가 포함된다.<br><br>
요청 Header는 요청한 URL, 메소드, 요청 생성에 사용된<br><br>
브라우저 및 기타 정보를 포함한다.
응답 Header는 컨텐츠에서 사용된 인코딩, 서버 시스템에서<br><br>
응답을 생성하는 데 사용되는 서버 소프트웨어 및 기타 정보를 포함한다.
</h3>
<h2><a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAyNDA4MDNfMzgg%2FMDAxNzIyNjczOTIwNjMz.lzvfzbWSY9SC2nQbfjUR21hHyw_saJpdA2EzS9ItrfIg.snbtbCvlixdkoafH0l3vAYGZ93v1h7oIjeKBz9ArEeUg.GIF%2F37A26339%25A3%25AD8F67%25A3%25AD4A6C%25A3%25AD87D7%25A3%25AD1B58FAD16C95%25A3%25DF20240803%25A3%25DF170833.gif&type=sc960_832_gif">감사합니다</a></h2>
