<h1>강의 정리</h1><h6>(저는 인프런에서 김영한 님의 <mark><a href="https://www.inflearn.com/course/%EA%B9%80%EC%98%81%ED%95%9C%EC%9D%98-%EC%9E%90%EB%B0%94-%EC%9E%85%EB%AC%B8?cid=332505">'김영한의 자바 입문 - 코드로 시작하는 자바 첫걸음'</a></mark>이라는 강의를 들었으므로 이 강의로 정리하겠습니다.)</h6><br><hr>
<h2><a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2F20131108_291%2Fcom7321_1383905922311X2Oho_JPEG%2F20131108_191555.jpg&type=sc960_832"><목차></a></h2><hr>
<h3>1. 주석<br><br>
2. 변수<br><br>
3. 연산자<br><br>
4. 조건문<br><br>
5. 반복문<br><br>
6. 스코프, 형변환<br><br></h3>
</목차><hr>
<h2>주석</h2>
<h3>주석은 아주 중요한 녀석이다.<br><br>
우리는 거의 모든 프로젝트를 혼자 하지 않는다.<br><br>
프로젝트도 팀플레이다.<br><br>
그래서 우리는 프로젝트를 할 때 자신의 코드가 어떤 방식으로 작동하는 지 써줘야 한다.<br><br>
하지만 프로젝트에서 소통을 어떻게 할까?<br><br><br><br>
그 방법 중 하나가 바로 주석이다.<br><br>
주석의 종류는 두 가지다.<br><br>
바로 '<b>한 줄 주석</b>'과 '<b>여러 줄 주석</b>'이다.<br><br>
한 줄 주석은 <mark>'//~~~'</mark> 이렇게 작성한다.<b><h4>(//이렇게 치면 컴퓨터는 못 알아본다.)</h4></b><br>
여러 줄 주석은  <mark>'/*~~~'</mark> 이렇게 작성 한다.<br><br>
여러 줄 주석을 할 때는 주석을 작성한 후 <mark>'~~~*/'</mark> 이렇게 닫아줘야 한다.<b><h4>(/*이렇게 치면<br> 컴퓨터는<br> 못 알아본다.*/)</h4></b><br><br>
</h3>
<h4>그런데 주석의 쓰임이 소통 말고도 한 가지 더 있다는 걸 아는가?<br><br>
주석은 오류를 찾을 때도 쓰인다.<br><br>
코드를 실행했을 때 오류가 나온다고 치자.<br><br>
이때 오류로 의심되는 코드를 주석처리한다.(이를 '코드를 잠근다'고 표현한다.)<br><br>
만약 코드가 오류 없이 실행된다면 주석처리한 코드에 오류가 있다는 것이다.<br><br>
<h3><a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAyMzA1MjVfMjMg%2FMDAxNjg0OTQ1NDY2OTM3.PmviJRkEiET99pFuIrVIEJhC4JSB09921-ineVqkgT0g.0LcdY61_jvWU-k7o2IyT638HCl9R4B1Zm9iWNzNNl4sg.JPEG.blossom_zze%2FP20230210%25A3%25DF191605000%25A3%25DFBC086ADE%25A3%25AD6425%25A3%25AD4ED4%25A3%25ADA417%25A3%25AD09B69AAE4E52.jpg&type=sc960_832">'주석 클리어!!'</a></h3>
</h4>
<hr>
<h2>변수</h2>
<h3>변수는 말 그대로 '<mark>변하는 수</mark>'다.<br><br>
(변수가 변하는 수라고 하지만, 변수에는 숫자, 문자, 문자열까지 많은 데이터가 들어갈 수 있다.)<br><br>
변수의 종류에는 정수(byte short, int, long), 실수(double, float), 불리언(boolean이라 쓰고 참, 거짓을 저장한다.), 문자 하나(char), 문자열('S'tring)<br><br><br>
그렇다면 변수라는 건 어떻게 만들까?<br><br>
변수를 만드는 행위를 '변수 선언'이라 한다.<br><br>
당신이 만야 숫자를 넣을 수 있는 변수를 만든다 하자.<br><br>
그럴 때 당신은 정수/실수, 수의 범위 등을 고려해야 한다.<br><br>
정수와 실수의 데이터형은 서로 다르며, 수의 범위에 따라서도 데이터형이 다르기 때문이다.<br><br>
주로 정수는 int, 실수는 double을 쓰며,<br><br>
정수에서 수의 범위가 -147~147에 해당한다면 byte, -32768~32767에 해당한다면 short, -2147483648~2147483647에 해당한다면 int,<br><br>
더 크면 long(-9223372036854775808~9223372036854775807)을 쓰고, 실수에서는 int와 범위가 같으면 float, long과 범위가 같으면 double을 쓴다.<br><br><br><br>
당신은 a 라는 int형 변수를 만들기로 했다.<br><br>
이제 당신은 a 라는 변수에 어떤 값을 넣을 지를 정해야 한다.<br><br>
이를 '변수 초기화'라 한다.<br><br>
당신은 a 에 200이라는 정수를 넣었다고 하자.<br><br>
이제 당신은 변수를 마스터 했다!<br><br>
이거 하나만 더 알면.<br><br>
변수를 선언할때는 규칙이 있는데,<br><br>
첫째, 변수 이름에 숫자를 첫 글자로 쓸 수 없다(나머지 자리는 가능)<br><br>
둘째, 이름에는 공백이 들어갈 수 없다.<br><br>
셋째, 예약어(ex. int, long과 같은 이미 기능이 정해져 있는 단어)를 변수 이름으로 사용할 수 없다.<br><br>
넷째, 변수에는 영문자, 숫자, 달러기호, 또는 밑줄만 사용할 수 있다.<br><br>
<h4>개발자 사이에서는 암묵적인 관례가 있는데 그 이름은 바로 '낙타표기법'이다.<br><br>
낙타표기법은 변수 이름이 여러 단어일때,<br><br>
첫 번째 단어는 소문자로 시작하고 그 이후의 각 단어는 대문자로 시작하는 방법이다. 자주 사용하여 익숙해지도록 하자.<br><br></h4>
<h3><a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAyMzAzMjVfMTgz%2FMDAxNjc5NzUyMjMzMjA1.IGXbCS4IALCShuUVIs96x-FpFzR-X_vZgFRqsFDyNHQg.pISTcHORxJ2KAhr_L71ifhTXFJw7FKmeJCeXhZr220Yg.JPEG.loivme%2F12222.jpg&type=sc960_832">'변수 클리어!'</a></h3>
<hr>
<h2>연산자</h2>
<h3>연산자는 계산을 할 때 쓰인다<br><br>
사칙연산을 수행하는 녀석이 연산자라고 생각하면 편하다.<br><br>
연산자에는 산술연산자, 증감연산자, 비교연산자, 논리연산자, 대입연산자, 삼항연산자가 있다.<br><br>
아까 말한 사칙연산 기호가 산술 연산자에 속한다.(+, -, *, /)<br><br>
이때, 컴퓨터에만 있는 연산이 하나 있는데,<br><br>
그건 바로 '나머지 연산'이다.<br><br>
나머지 연산을 하면 나눗셈을 할때 나머지만 출력한다.<br><br>
나머지 연산자는 '%'다.<br><br>
나머지도 나눗셈의 일종이므로 '%'도 산술연산자에 들어간다.<br><br><br>
증감 연산자는 1씩 늘리고 줄일때 사용한다.<br><br>
정수형 변수 a 가 있을때 a++는 a에 1을 더하는 코드다.<br><br><br>
비교 연산자는 말 그대로 두 값을 비교할때 쓰인다(같다, 아니다, 이상, 이하, 초과, 미만)<br><br>
이때 같다/아니다를 표현할때는 같다(==)와 아니다(!=)로 표현하고,<br><br>
크고 작음을 판별할때는 부등호가 먼저온다(이상(>=), 이하(<=), 초과(>), 미만(<))<br><br><br>
논리연산자는 이 코드가 논리적으로 참인지 거짓인지를 판별한다.<br><br>
논리 연산자에는 둘 다 참이어야 참을 출력하는 &&(그리고),<br><br>
하나만 참이어도 참을 출력하는 ||(또는),<br><br>
참/거짓을 반대로 출력하는 !(아니다)가 있다.<br><br><br>
대입연산자는 변수에 값을 대입할 때 사용하는 연산자다.<br><br>
변수에 값을 대입할때는 대부분 '='을 쓴다.<br><br>
하지만 정수 a라는 변수에 a+1이라는 값을 넣는다 치자.<br><br>
코드로 작성하면<br><br>
a = a+1<br><br>
이라는 코드가 나온다.<br><br>
프로그래밍은 반복을 피한다.<br><br>
그래서 이 코드는 줄일 수가 있다.(a라는 변수가 반복되므로)<br><br>
코드를 줄이면<br><br>
a += 1<br><br>
이라는 코드가 나온다.<br><br>
이때 +=도 대입연산자다.<br><br>
a+1에서 '+'는 산술연산자이므로<br><br>
대입연산자는 '산술연산자'+'='으로 쓸 수도 있다.<br><br>
삼항 연산자는 이 다음 챕터인 '조건문'과 밀접한 관련이 있어 '조건문'에서 배우도록 하겠다.<br><br><br>
<a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAyNDA3MTJfMTQ4%2FMDAxNzIwNzkyMzM4NDM3.CRAV66x5c5h7TBEg6HDxQUvZtwqX4Elt9jU2Wss-TUUg.0vVeDrXhsTqhKh7Wy04Ms7rNADWXN6JC0kpHYEzQqgYg.JPEG%2FIMG_3646.jpg&type=sc960_832">'연산자 클리어!'</a></h3>
<h2>조건문</h2>
<h3>조건문은 조건이 참인지 거짓인지 판별하는 코드다.</h3>
