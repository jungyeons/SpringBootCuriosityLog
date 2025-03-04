# 📂 **SpringBootCuriosityLog**  
📚 **Spring Boot 공부 중 생긴 질문과 답변을 정리한 저장소**  

**SpringBootCuriosityLog**에 오신 것을 환영합니다!  
이 저장소는 Spring Boot를 공부하면서 생긴 질문들을 기록하고, 그에 대한 답변을 정리한 Q&A 형식의 자료입니다. 기초적인 내용부터 고급 주제까지, Spring Boot의 "왜?"와 "어떻게?"를 탐구하는 데 도움이 될 것입니다.  

---

## 🌟 목적  

이 저장소는 다음을 목표로 합니다  
1. Spring Boot에 대한 **질문과 답변 모음**을 제공합니다.  
2. 학습 과정을 기록하고 이해를 심화시킬 수 있는 **개인 학습 로그**로 활용됩니다.  
3. 비슷한 궁금증을 가진 사람들에게 **도움이 되는 자료**를 제공합니다.  

---

## 🛠️ 사용 방법  

1. **질문 탐색하기**  
   질문은 카테고리별로 나누어져 있습니다. 각 질문에는 상세한 설명과 필요한 경우 참고 자료가 포함되어 있습니다.  

2. **기여하기**  
   새로운 질문이나 답변을 추가하고 싶으신가요? Pull Request를 통해 자유롭게 기여할 수 있습니다. 함께 성장하는 지식의 장을 만들어 봅시다!  

---

## 🗂️ 예상 되는 내용들  

1. **핵심 개념**  
   - Spring Boot란 무엇인가요?  
   - `@RestController`와 `@Controller`의 차이는 무엇인가요?  
   - 의존성 주입(Dependency Injection)은 어떻게 작동하나요?  

2. **고급 주제**  
   - Spring Boot에서의 AOP(Aspect-Oriented Programming) 개념  
   - Spring Security를 활용한 인증 및 권한 관리  
   - RESTful API 설계 원칙  

3. **추가 주제**  
   - Spring Boot에서의 데이터베이스 연결 방법은?  
   - 프로파일(Profile) 설정을 통한 환경별 구성 관리  

---

## 🤝 기여 방법  

이 저장소에 기여하고 싶다면 다음을 참고하세요:  
1. **질문 제출하기**  
   새로운 Spring Boot 관련 질문을 Issue로 남겨주세요.  
2. **답변 추가하기**  
   기존의 질문에 대한 답변을 개선하거나, 새로운 답변을 추가해주세요.  
3. **저장소 개선하기**  
   카테고리 분류, 태그 추가, 검색 기능 등 새로운 아이디어를 제안하고 구현해주세요.  

---

## 📝 예시 Q&A  

### Q: **Spring Boot란 무엇인가요?**  
**A:**  
- Spring Boot는 Spring 프레임워크를 기반으로 하여 애플리케이션 개발을 간소화하고 신속하게 할 수 있도록 도와주는 도구입니다. 기본 설정 및 구성을 자동으로 처리하여 개발자가 비즈니스 로직에 집중할 수 있게 합니다.

   ```java
   // Spring Boot 애플리케이션 시작 예제
   import org.springframework.boot.SpringApplication;
   import org.springframework.boot.autoconfigure.SpringBootApplication;

   @SpringBootApplication
   public class MyApplication {
       public static void main(String[] args) {
           SpringApplication.run(MyApplication.class, args);
       }
   }
   ```

---

## 📌 라이선스  

이 저장소는 [MIT 라이선스](LICENSE)에 따라 사용됩니다
