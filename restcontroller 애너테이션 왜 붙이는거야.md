<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# 

---

# restcontroller 애너테이션 왜 붙이는거야

`@RestController` 애너테이션은 Spring Framework에서 RESTful 웹 서비스를 쉽게 개발하기 위해 제공되는 애너테이션입니다. 이 애너테이션을 사용하는 이유는 다음과 같습니다:

### **1. RESTful 웹 서비스 개발에 최적화**

`@RestController`는 `@Controller`와 `@ResponseBody`를 결합한 형태로, 메서드의 반환값이 HTTP 응답 본문으로 직접 전달됩니다. 즉, JSON이나 XML 같은 데이터 형식으로 응답을 반환하는 RESTful API를 개발할 때 매우 간편하게 사용할 수 있습니다[^1][^3][^7].

### **2. 간소화된 코드**

- `@ResponseBody`를 메서드마다 붙일 필요가 없습니다. `@RestController`를 클래스 레벨에 선언하면 해당 클래스의 모든 메서드가 자동으로 HTTP 응답 본문에 데이터를 반환하도록 설정됩니다[^3][^4].
- 데이터 객체를 반환하면 Spring이 이를 자동으로 JSON 또는 XML로 직렬화하여 클라이언트에게 전달합니다[^5][^7].


### **3. HTML 뷰 대신 데이터 반환**

- `@Controller`는 주로 HTML 뷰를 반환하기 위해 사용되며, 뷰 리졸버(View Resolver)를 통해 렌더링된 페이지를 클라이언트에게 제공합니다.
- 반면, `@RestController`는 HTML 뷰 대신 데이터(주로 JSON)를 반환합니다. 이는 RESTful API에서 클라이언트와 서버 간 데이터 교환을 위해 설계된 방식입니다[^1][^6].


### **4. REST 아키텍처 스타일 지원**

REST(Representational State Transfer)는 자원을 중심으로 설계된 아키텍처 스타일입니다. `@RestController`는 이러한 RESTful 웹 서비스의 컨트롤러로 사용되며, 클라이언트 요청에 따라 자원에 대한 CRUD(Create, Read, Update, Delete) 작업을 수행하는 데 적합합니다[^2][^5].

### **사용 예시**

```java
@RestController
public class MyRestController {

    @GetMapping("/api/hello")
    public String hello() {
        return "Hello, World!";
    }
}
```

위 코드에서 `/api/hello` 요청은 단순한 텍스트 응답("Hello, World!")을 JSON 형식으로 반환합니다.

### **결론**

`@RestController`는 RESTful API 개발을 단순화하고 직관적으로 만들어주는 강력한 도구입니다. 데이터를 주고받는 API를 설계할 때 `@RestController`를 사용하면 코드가 간결해지고 유지보수가 쉬워집니다.

<div style="text-align: center">⁂</div>

[^1]: https://igventurelli.io/understanding-the-differences-between-controller-and-restcontroller-annotations/

[^2]: https://curiousjinan.tistory.com/entry/Spring-Boot-REST-Controller-Usage-Understanding-RestController

[^3]: https://kang-james.tistory.com/entry/스프링-Controller와-RestController의-차이를-알고있나요

[^4]: https://codingnomads.com/spring-restcontroller-endpoints

[^5]: https://dorothy-koo.gitbooks.io/springboot/content/chapter1.html

[^6]: https://www.devkobe24.com/Spring/2024-09-24-Controller-DTO-APIspec-GetMapping-MIME-RequestParam-Formdata-RestController.html

[^7]: https://mangkyu.tistory.com/49

[^8]: https://sunghyun98.tistory.com/299

[^9]: https://www.baeldung.com/spring-controller-vs-restcontroller

[^10]: https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/web/bind/annotation/RestController.html

[^11]: https://hongs-coding.tistory.com/127

[^12]: https://wikidocs.net/237052

[^13]: https://observerlife.tistory.com/8

[^14]: https://velog.io/@leesomyoung/Spring-Boot-RestController와-Controller의-특징과-차이점

[^15]: https://velog.io/@oyeon/RestController-개념

[^16]: https://docs.spring.io/spring-framework/reference/web/webmvc/mvc-controller.html

[^17]: https://velog.io/@wlsdks12/Spring-MVC-RestController

[^18]: https://suzuworld.tistory.com/116

[^19]: https://congsong.tistory.com/28

[^20]: https://takimon.tistory.com/31

