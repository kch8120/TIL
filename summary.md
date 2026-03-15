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
이때 문자(열)에도 연산을 사용할 수 있는데,
문자열1 + 문자열2를 하면 문자열1문자열2가 나오고,
문자열3 + 정수를 하면 문자열1정수가 나오고,
문자열4*정수를 하면 문자열4를정수번출력한다.
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
  <hr>
<h2>조건문</h2>
<h3>조건문은 조건이 참인지 거짓인지 판별하는 코드다.<br><br>
조건문의 판단에 따라 코드가 완전히 바뀔 수 있다.<br><br><br>
예를 들어 조건이 '나이가 18세 인 경우'라 하자<br><br>
18세 이상이 아니면 '미성년자'를 출력하고<br><br>
18세 이상이라면 '성인'을 출력하는 것이다.<br><br><br>
이때 조건문이 '나이가 18세 이상'이고,<br><br>
참일 때 결과가 '성인',<br><br>
거짓일 때 결과가 '미성년자'인것이다.<br><br><br>
이런 조건문을 쓸 때는 'if-else'라는 녀석을 쓴다.<br><br>
위에서 쓴 조건문을 if를 이용하면<br><br><br>
int age = 18;

if (age>=18) { <-조건문의 시작과 끝은 항상 중괄호다!!<br><br>
  (출력하려면 이 코드를 작성한다!!--)  System.out.println('성인');  (코드에서는 세미콜론으로 줄을 구분한다 <br><br>
} else {<br><br>
  System.out.println('미성년자')<br><br>
}<br><br>
이렇게 쓸수 있다.<br><br><br>
이때 조건이 여러개인 경우가 있다.<br><br><br>
ex. 학력을 판별하는경우<br><br>
7세이하 미취학<br><br>
8세이상 13세이하 초딩<br><br>
14세이상 16세이하 중딩<br><br>
17세이상 19세이하 고딩<br><br>
20세이상 성인<br><br>
이럴 때는 어떻게 할까?<br><br><br>
바로 'else if'를 쓰는거다.<br><br>
첫 번째 조건은 if, <br><br>
두 번째 조건부터는 else if,<br><br>
마지막 조건에는 else를 쓰면 된다.<br><br><br>
하지만 조건문간의 관계가 없는 경우(조건1을 만족했다고 해서 조건2를 만족하면 안되는 이유가 없는 경우)<br><br>
else와 else if 없이 if만 쓸 수 있다.<br><br><br>
ex. 할인 하는 경우<br><br>
조건 1을 만족하면 쿠폰 1을 주고,<br><br>
조건 2를 만족하면 쿠폰 2를 준다 하자.<br><br>
이때 쿠폰은 중복할인이 가능하다.<br><br>
이런 경우에는 if만 쓴다(else를 쓰지 않는다)<br><br><br>

그런데 만약 당신이 어떤 변수에 관해 조건문을 쓴다 하자.<br><br>
변수의 값이 정해져있다면 당신은 새로운 조건문을 쓸 수가 있다.<br><br>
바로 switch 문이다.<br><br><br>
당신이 이번엔 회원 등급에 따라 쿠폰을 뿌린다고 하자.<br><br>
이때 switch 문을 쓰면<br><br>
int  grade = 1;<br><br>
int coupon;<br><br>
switch(grade) {<br><br>
&nbsp;&nbsp;case 1:<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;coupon = 5000;<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;break; (--조건을 만족했으면 메모리 사용을 줄이기 위해 break(깨다)를 이용해 조건문을 탈출한다)<br><br>
&nbsp;&nbsp;case 2:<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;coupon = 2000;<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;break;<br><br>
&nbsp;&nbsp;case 3:<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;coupon = 1000;<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;break;<br><br>
&nbsp;&nbsp;&nbsp;default:<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;coupon = 500;<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;break;<br><br>
}<br><br>
System.out.println("발급받은 쿠폰 " + coupon);<br><br><br>
그런데 개발자들은 switch문을 더 쉽고 간편하게 쓰기 위해 개조를 시켰다(?)<br><br>
위 코드를 개조된 switch문으로 만들어 보겠다.<br><br>

int  grade = 1;<br><br>

int coupon = switch(grade) {<br><br>
&nbsp;&nbsp;case 1 -> 5000;<br><br>
&nbsp;&nbsp;case 2 -> 2000;<br><br>
&nbsp;&nbsp;case 3 -> 1000;<br><br>
&nbsp;default -> 500;<br><br>
};<br><br>
System.out.println("발급받은 쿠폰 " + coupon);<br><br>
이렇게 쓸 수가 있다.<br><br><br>

이제 드디어 삼항 연산자다!!<br><br>
삼항연산자는 말 그대로 세 개의 항으로 이루어져 있는 조건문이다.<br><br>
구조는 '조건 ? 참 : 거짓' 이다.<br><br><br>
아까 본 나이 조건문을 다시 사용하겠다.<br><br>
int age = 18;<br><br>
String status = if (age >=18) ? "성인" : "미성년자";<br><br>

System.out.println(status);<br><br>

이렇게 쓰면 코드가 엄청 간단해진다 ㄷㄷ<br><br></h3>

<h3><a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAyMTEyMjBfMTYz%2FMDAxNjM5OTkyOTE1OTU0.2iT4DbiooRTwOOiAexmK9HcajaXr6ucr944TUBTmwi0g.-P1THdN0LJwpCa8GmvMGyaEkWIylp_ojt6BPvfXjK5kg.JPEG.yjun03165%2FIMG_8050.JPG&type=sc960_832">'조건문 클리어!'</a></h3>
<hr>
<h2>반복문</h2>
<h3>
반복문은 같은 코드를 반복할 때 쓰인다.<br><br>
반복문은 크게 while문과 for문 두 가지로 나뉜다.<br><br>
while문은 조건에 따라 코드를 반복해서 실행할 때 사용한다.<br><br>
while문은 조건식을 확인해 참이면 코드 블록을 실행하고, 거짓이면 while문을 벗어난다.<br><br>
코드 블록을 실행한 다음에는 다시 조건식을 확인하고 참/거짓일때 결과를 실행한다.<br><br>
ex. 숫자를 하나씩 3번 더하는 경우<br><br>
int sum = 0;<br><br>
int count = 0;<br><br>
while (count < 3) {<br><br>
&nbsp;&nbsp;count += 1;<br><br>
&nbsp;&nbsp;sum += 1;<br><br>
System.out.println(sum);<br><br>
}<br><br>
의 출력 결과는 3이다.<br><br><br>
sum과 count는 처음에 0으로 변수 초기화를 진행한다.<br><br>
0<3이므로 count와 sum에 1을 더한다.<br><br>
1<3이므로 count와 sum에 1을 더한다.<br><br>
2<3이므로 count와 sum에 1을 더한다.<br><br>
3<3은 거짓이므로 while문을 빠져나온다.<br><br>
sum을 출력한다.<br><br>
while문은 조건을 만족해야 코드를 실행하지만,<br><br>
일단 코드를 한 번 실행하고 그 다음에 조건을 검사하는 경우가 있다.<br><br><br>
그건 바로 do-while문이라 한다.<br><br>
int i = 10;<br><br>

while( i < 3) {<br><br>
&nbsp;&nbsp;System.out.println(i);<br<br>
&nbsp;&nbsp;i++;<br><br>
}
원래 이 코드는 조건식을 만족하지 않아 실행되지 않지만,<br><br><br>
int i = 10;<br><br>

do{<br><br>
&nbsp;&nbsp;System.out.println(i);<br><br>
&nbsp;&nbsp;i++;<br><br>
} while( i < 3);<br><br>
이렇게 작성하면 조건식을 만족하지 않아도 한 번은 실행하므로 10이라는 결과가 나온다.<br><br><br>
while문을 이용하면 무한반복문을 만들 수 있는데,<br><br>
작성 방법은 while(true)를 사용하면 된다.<br><br>
조건식이 항상 참이므로 이 코드는 무한반복된다.<br><br><br>
그렇다면 어떻게 벗어날까?<br><br>
바로 break와 continue다.<br><br>
while문 안에서 break를 만나면 while문 자체가 멈추고,<br><br>
continue를 만나면 while문안의 나머지 코드는 무시하고 다음 반복으로 넘어간다.<br><br>
<h5>break와 continue를 사용하지 않으면 코드가 멈추지 않는다..ㄷㄷ</h5><br><br><br>
<h3>이제 다음은 for문이다.<br><br>
for문은 주로 반복 횟수가 정해져 있는 경우에 사용한다.<br><br>
for문의 구조는 for (초기식 ; 조건식 ; 증감식) {<br><br>
&nbsp;&nbsp;코드<br><br>
}<br><br>
이렇게 이루어져있다.<br><br<br>>
초기식이 실행되고 조건식을 검사한다.<br><br>
조건식이 참이면 코드가 실행되고, 거짓이면 ,for문을 빠져나온다.<br><br>
코드가 종료되면 증감식을 실행하고, 다시 조건식을 검사한다.<br><br><br>
ex.1부터 10까지 출력하는 경우<br><br>
for (int i = 1; i <= 10; i++) {<br><br>
&nbsp;&nbsp;System.out.println(i);<br><br>
}<br><br>
이렇게 쓰면 된다.<br><br>
i는 1로 초기화되고,<br><br>
1<=10이므로 i를 출력한다<br><br>
i에 1을 더한다.<br><br>
.<br>
.<br>
.<br>
10<=10이므로 i를 출력한다.<br><br>
i에 1을 더한다.<br><br>
i는 10보다 크므로 for문을 빠져나간다.<br><br><br>

반복문은 반복문 안에 또 있을 수 있는데,<br><br>
이를 중첩 반복문이라 한다.<br><br>
for문으로 예시를 들어보자.<br><br>
for (int i = 0; i < 2; i++) {<br><br>
&nbsp;&nbsp;for(int j = 0; j < 3; j++) {<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;System.out.println(j);<br><br>
&nbsp;&nbsp;}<br><br>
}<br><br>
이렇게 작성하면 j가<br><br>
1<br>
2<br>
3<br>
1<br>
2<br>
3<br>
이렇게 나온다.<br><br>
1 2 3을 출력하고 다시 위로 올라가 1 2 3을 출력하는 것이다.<br><br>


<h3><a href="https://search.pstatic.net/common/?src=http%3A%2F%2Fblogfiles.naver.net%2FMjAxOTA3MjFfMTkx%2FMDAxNTYzNzE0Mzk2MTI5.I0ftk0oShJTX-ZaN2AtpBjAX8HlyveuIrOmWFifymFEg.yEweFNmXdpG-GsyErfIOSrMYUovUtsHiIYeGWZS8aD4g.GIF.parkamsterdam%2FIMG_1829.GIF&type=sc960_832_gif">'반복문 클리어!'</a></h3></h3>
<hr>
<h2>스코프, 형변환</h2>
지금까지 우리가 사용한 변수는 지역변수다.
지역변수는 이름 그대로 특정 지역에서만 사용할 수 있는 변수라는 의미다.
지역변수는 그 지역을 벗어나면 사용할수 없다.
여기서 말하는 지역이란 블록을 의미한다.({
})
이런 걸 블록이라 한다.
예를 들어 당신이 if문 안에 int a라는 변수를 만들었다 치자.
그럼 그 변수는 if문 밖에서는 쓸 수 없다는 뜻이다.
여기서 a의 생존범위는 if문이 된다.
이런 생존범위를 '스코프'라 한다.
그렇다면 개발자들은 왜 굳이 스코프를 만들어서 우리의 머리를 아프게 하는걸까?
그 이유는'메모리 최소화와 단순한 코드 추구'에 있다.
우선 변수가 모든 블록에 살아있으면 그 변수를 쓰지 않더라도
메모리는 그걸 다 고려해야 하므로 메모리가 낭비된다.
그리고 개발자들에게 좋은 코드란 단순한 코드를 의미한다.
변수가 모든 블록에 살아있으면 코드가 복잡해진다고 보는 것이다.
그래서 개발자들은 지역변수 라는 개념을 만들었다.

우리가 숫자 변수를 선언한다 하자.
숫자변수는 int, long, double이 있다.
오른쪽으로 갈 수록 큰 범위이다.
그렇다면 int에 있는 숫자와 long에 있는 숫자가 서로 바뀔 수 있을까?
결론은, 된다.
그게 바로 형변환이다.
int에 있는 숫자를 long에 넣을 때는 아무 문제 없이 자동으로 형변환이 된다.(long이 더 크니까)
우리는 이걸 자동형변환(묵시적형변환)이라 한다.
long에 있는 int 범위 내 숫자를 int에 넣을 때도 자동형변환이 일어난다.
하지만 long에 있는 int 범위 외 숫자를 int에 넣을 때는 오류가 발생한다.(컴파일러 오류)
아까는 된다고 했으면서..
권채혁이 거짓말을 한것일까?
거짓말은 아니다.
다만 바꾸려면 절차가 좀 더 필요하고 정확성이 떨어질 뿐이다.
예를 들어보자.
double에 있는 0.1이 있다.
이걸 int에 넣으면 0이 된다.
실수에서 정수로의 형변환에서는 소수점이 버려진다.(반올림 아님!)
double에 있는 2147483648을(int 최대범위 +1값)
int에 넣으면 -2147483648이 된다.(int 최소범위)
최대범위를 넘어서면 최소범위에서 다시 시작한다.
시계를 생각하면 편하다.
최대범위인60분에서 1분이 더 지나면
최소범위인 0분에서 +1을 해 1분이 되는 것이다.
이렇게 큰 범위에서 작은 범위에 값을 넣는 행위를 '명시적 형변환'이라 한다.
명시적 형변환은 숫자 앞에 바꾸고 싶은 범위를 쓰면 된다.
ex. double 2147483648을 int에 넣을 때
double a = 2147483648
int b = (int) a
일때 b를 출력하면 -2147483648이 나온다.
