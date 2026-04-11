### 우리는 Spring이 개발자들을 위한 framework라는 것을 배웠다.
### Spring MVC란 웹 계층에 서블릿 API를 기반으로
### 클라이언트의 요청을 처리하는 모듈이 있는데
### 이를 Spring MVC라 한다.
## 그렇다면 MVC 패턴이 뭘까?
### 이건 개발자에게 어떤 게 좋은 걸까?
### 알아보자.
### <img src="https://velog.velcdn.com/images/choidongkuen/post/1e74c8da-4e1b-400e-93d5-391034a2d49b/image.png">
### 결론부터 말하면 MVC 패턴은 애플리케이션을 개발할 때 사용하는 디자인 패턴이다.
### 앱의 개발 영역을 위 사진처럼 MVC(Model, View, Controller)로 구분하는 것이다.
### MVC 패턴을 도입하면서 UI영역과 도메인(비즈니스 로직) 영역으로 구분되어
### 서로에게 영향을 주지 않으면서 개발과 유지보수가 가능하게 되었다.
```
@Controller // Controller 클래스 -> 빈 객체로 등록
public class HelloController {

	@RequestMapping("/hello.do") // 매핑할 URL
    public String hello(Model model) {  
    	
        model.addAttribute("greeting", "안녕하세요"); // Model에 데이터를 설정
        return "hello"; // 리턴할 View 이름
   }
}
```
- ### Model
  #### Spring MVC 기반의 웹 애플리케이션이 클라이언트의 요청을 전달받으면
  #### 요청 사항을 처리하기 위한 작업을 한다.
  #### 처리한 작업의 결과를 클라이언트에게 돌려주어야 하는데,
  #### 이때 돌려주는 결과 데이터를 Model이라 한다.
- ### View
  #### Model을 이용하여 웹 애플리케이션의 화면에 보이는 리소스를 제공한다.
  #### Spring MVC에는 다양한 View 기술이 포함되어 있다.
        1. HTML 페이지 출력
        2. PDF, Excel 등의 문서 형태로 출력
        3. XML, JSON 등 특정 형식의 포맷으로 변환
- ### Controller
  #### 클라이언트 측의 요청을 직접적으로 전달받아
  #### Model과 View의 중간에서 상호작용을 해주는 역할을 한다.
  #### 클라이언트 측의 요청을 전달받아 비즈니스 로직을 거친 후,
  #### Model 데이터가 만들어지면 이 데이터를 View로 전달하는 역할을 한다.

### Spring MVC 패턴 구조
### <img src="https://velog.velcdn.com/images/choidongkuen/post/04e2d8a0-5bcf-4dbe-b430-420d4bad9f11/image.png">
### MVC 패턴에는 다양한 종류가 있지만, 보통 위의 이미지를 기반으로 한
### MVC 패턴을 Spring MVC 패턴이라고 한다.
- ### DispatcherServlet
  #### 클라이언트의 요청을 전달받는다.
  #### Controller에게 요청을 전달하고,
  #### 컨트롤러가 리턴한 결과값을 View에 전달한다.
  #### DispatcherServlet은 컨트롤러의 컨트롤러이기 때문에
  #### 프론트 컨트롤러라고도 불린다.
- ### HandlerMapping
  #### 클라이언트의 요청 URL을 어떤 컨트롤러가 처리할지 결정하는 기능을 한다.
- ### Controller
  #### 클라이언트의 요청을 처리한 뒤, 결과를 리턴한다.
  #### 응답 결과에서 보여줄 데이터를 Model에 담아 전달한다.
  #### Controller에서 나오는 Model은 ModelAndView로 변환된다.
- ### ModelAndView
  #### Controller에서 처리한 결과 정보 및 View 선택에 필요한 정보를 담는다.
- ### ViewResolver
  #### ModelAndView를 전달받은 DispatcherServlet은 실제 클라이언트에게
  #### 보여질 View를 렌더링하기 위해 어떤 View 객체를 사용할지 결정하기 위해
  #### ViewResolver를 호출한다.
- ### View
  #### ViewResolver에 의해 View 객체가 결정되고 해당 객체를 통해
  #### View를 렌더링한다.
### Spring MVC 패턴의 장점과 단점
- ### 장점
    1. #### Model, View, Controller로 나누어서 개발을 할 수 있기에 역할 분담이 가능하다.
    2. #### 중복된 코드를 줄일 수 있고, 확장성 있고 유연한 코딩이 가능하다.
    3. #### 각 분야로 나누어져있기 때문에 디버깅과 테스팅이 용이하다.
- ### 단점
    1. #### 프로젝트의 규모가 커지면 복잡해질 수 있다. 즉, 너무 많은 파일이 생성될 수 있다.
    2. #### 하나의 파일을 여러 파일로 나누어서 개발하기 때문에 유지보수 시간이 길어질 수 있다.



## 웹 계층 구조
1. ### 프레젠테이션 계층(presentation layer)
    - #### HTTP 요청을 받고 이 요청을 비즈니스 계층으로 전송하는 역할을 한다
    - #### Controller가 이 계층의 역할을 한다.
2. ### 비즈니스 계층(Business layer)
    - #### 핵심 업무 로직의 처리 방법 기술과 관련 데이터의 적합성을 검증한다.
    - #### 트랜잭션을 관리 및 처리한다.
    - #### 프레젠테이션 계층과 데이터 액세스 계층 사이를 연결하는 역할을 한다.
    - #### Service가 이 계층의 역할을 한다.
3. ### 퍼시스턴스 계층(Persistence layer)
    - #### 모든 데이터베이스 관련 로직을 처리한다(CRUD).
    - #### 데이터베이스에 접근하는 DAO 객체를 사용할 수 있다.
    - #### Repository가 이 계층의 역할을 한다.
4. ### DTOs(Data Transfer Object)
    - #### 다른 계층 간 데이터 교환을 위한 객체이다.
    - #### 로직을 갖지 않고 getter나 setter 메소드를 가진다.
5. ### 도메인 모델 계층(Domain Model layer)
    - #### 각 계층 사이에 전달되는 실질적인 비즈니스 객체이다.
    - #### 비즈니스 로직을 처리하는 영역이다.
    - #### Entity나 VO가 해당된다.
### 비즈니스 로직은 도메인 모델 계층에 작성한다.
- #### 비즈니스 계층은 다양한 Model을 읽어 제공하기 때문에 복잡도가 매우 높아진다.
    - #### 이때 복잡도를 낮추기 위해 비즈니스 로직을 도메인모델 계층으로 이동시키고
    - #### 비즈니스 계층에서는 처리 방법 등을 기술한다.
### 관련 용어
### DTO(Data Transfer Object)
- #### 순수하게 데이터를 담아 계층간으로 전달하는 객체
- #### 로직을 갖고있지 않으며 getter, setter만을 가짐
- #### 유지보수를 유연하게 할 수 있음
### VO(Value Object)
- #### 값 그 자체를 나타내는 객체
- #### 객체 주소가 달라도 필드값이 같다면 두 객체를 같은 객체로 봄
- #### 로직을 포함할 수 이으며 생성자를 사용해야 함
### DAO(Data Access Object)
- #### DB에 접근하는 객체, DB를 사용해 데이터를 조작하는 기능을 하는 객체이다.
- #### Repository라고도 부른다.
- #### 비즈니스계층과 DB를 연결하는 역할을 한다.
### <img src="https://velog.velcdn.com/images/recordhyo/post/505ae121-a18c-4208-adef-1e4ae2ca987f/image.png">