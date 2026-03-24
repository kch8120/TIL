# HTTP
## <a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2F20131108_291%2Fcom7321_1383905922311X2Oho_JPEG%2F20131108_191555.jpg&type=sc960_832"><목차></a><hr>
<h2>
- HTTP가 뭘까?<br>
- HTTP Method가 뭘까?<br>
- HTTP Status code가 뭘까?<br>
- HTTP의 무상태성이 뭘까?</h2>
<hr>
<h2>HTTP가 뭘까?<br><br></h2>
<h3>
HTTP는 <mark>HyperText Transfer Protocol</mark> 약자이다.<br><br>
뜻은 하이퍼텍스트 전송 규약이다.<br><br>
그런데 우리가 못봤던 단어가 있다.<br><br>
하이퍼텍스트가 뭘까?<br><br>
하이퍼텍스트는 하이퍼링크와 비슷한 개념이다.<br><br>
단지 하이퍼링크를 좀 더 고급지게 개조시킨 것이 하이퍼텍스트인 것이다.<br><br>
HTTP는 기본적으로 <mark>클라이언트-서버</mark> 모델을 사용하는 요청-응답 기반 프로토콜이다.<br><br>
클라이언트가 뭔가를 요청하면, 서버가 응답하는 과정에서 사용되는 프로토콜이 HTTP인 것이다.<br><br><br>
예를 들어 웹사이트에 방문해서 영상을 보거나, 스마트폰으로 앱을 사용하거나,<br><br>
브라우저로 데이터를 업로드할 때 클라이언트는 서버에 HTTP 요청 메시지를 보낸다.<br><br><br>
그럼 HTML 파일, 이미지, 동영상 같은 콘텐츠 리소스를 제공하는 서버는<br><br>
클라이언트에 응답 메시지를 회신한다.<br><br></h3>
<h2>
HTTP Method가 뭘까?<br><br></h2>
<h3>
이 응답에는 완료 상태, 요청받은 콘텐츠 관련 정보들이 포함되어 있다.<br><br>
HTTP가 하는 응답에는 그 안에 포함된 데이터를 설명하는 HTTP 헤더가 추가로 달려 있다.<br><br>
이 헤더는 유저에게는 보이지 않지만, 브라우저와 서버는 바로 이 HTTP 헤더로 정보를 읽는다.<br><br>
헤더와 함께 요청한 결과를 표시하는 HTTP 상태 코드를 전달하기도 하는데,<br><br>
이 상태 코드의 예시는 다음과 같다.<br><br>
<mark>200=성공<br><br>
301=영구 이동(리디렉션)<br><br>
404=찾을 수 없음<br><br>
451=법적인 이유로 사용 불가<br><br>
500=내부 서버 오류<br><br></mark>
여기서 가장 대표적인 코드는 바로 404 코드로<br><br>
인터넷을 사용할 때 <ins>404 not found</ins> 모습으로 흔히 나타나며<br><br>
404 오류라고도 부릅니다.<br><br></h3>