### 📕 스프링?
**스프링**은 특정한 하나가 아닌, 여러가지 기술들의 모음이다.
ex) 스프링, 스프링부트, 스프링데이터, 세션, 시큐리티, Rest Docs ...    
[스프링](https://spring.io/)에서 다른 기술들에 관한 공식문서를 알아 볼 수 있다.

### 📕 스프링의 핵심
스프링은 자바 기반의 프레임 워크이다.
자바의 가장 큰 특징은 **객체 지향 언어**라는 점인데, 스프링은 자바의
**좋은 객체 지향** 애플리케이션 개발을 도와주는 프레임워크이다.

### 📕 +) API, Library, Framework
**API**는 시스템이나 애플리케이션 간 서로 정보 교환하는데 사용하는 약속이다.
이를 통해 다른 애플리케이션과 통신 혹은 데이터를 주고 받는다.

**Library**와 **Framework**는 개발자들이 사용하기 좋게 만들어 놓은 코드 조각 모음이다.
그러나 **Framework**는 **"프레임"**이라는 말 그대로 틀을 만들어 두고
개발자로 하여금 사용 방법을 강제하고, **Library**는 개발자가 좀 더 자유롭게 사용 할 수 있는 코드 조각 모음이다.

### 📕 좋은 객체 지향
- 프로그램을 유연하고 변경이 용이하게 만들어야 한다. (역할과 구현 분리)
- **역할과 구현**으로 구분하면 단순해지고, 유연해지며, 변경도 편리해진다.
역할(인터페이스), 구현(인터페이스를 구현한 클래스, 구현 객체)
- **다형성(Polymorphism)**을 지키는 것이 중요하다.
**다형성의 본질** - 클라이언트를 변경하지 않고, 서버의 구현 기능을 유연하게
변경할 수 있다.

즉, **좋은 객체 지향**은 인터페이스를 안정적으로 잘 설계하는 것이 중요하다.

### 📕 스프링과 객체 지향의 연관성
**다형성(Polymorphism)** 이 가장 중요하다.
스프링은 다형성을 극대화해서 이용할 수 있게 도와주는 프레임워크이다.

### 📕 좋은 객체지향 설계의 5가지 원칙 (SOLID)
- SRP : 단일 책임 원칙 (Single Responsibility Principle)
- OCP : 개방 - 폐쇄 원칙 (Open / Closed Principle)
- LSP : 리스코프 치환 원칙 (Liskov Substitutuin Principle)
- ISP : 인터페이스 분리 원칙 (Interface Segregation Principle)
- DIP : 의존관계 역전 원칙 (Dependency Inversion Principle)

**OCP와 DIP**가 가장 중요하다.
- **OCP** : 소프트웨어 요소는 **확장에는 열려있으나 변경에는 닫혀 있어야한다**.
- **OCP의 문제점** : 구현 객체를 변경하려면 클라이언트 코드를 변경해야 한다.
ex) memberService에서 MemoryRepo를 JdbcRepo로 바꾸려면 코드 변경이 필요하다. 다형성을 사용했지만 OCP원칙을 지킬 수 없게됨.
**해결** : 객체를 생성하고, 연관관계를 맺어주는 별도의 조립, 설정자가 필요
**이를 스프링 컨테이너가 해결해준다.**

- **DIP** : "추상화에 의존해야지, 구체화에 의존하면 안된다"는 원칙을 따르는 방법 중 하나이다.
즉, 구현 클래스에 의존하지 말고, 인터페이스에 의존하라는 뜻

### 📕 객체 지향 설계와 스프링
스프링은 DI (Dependency Injection) : 의존관계, 의존성 주입, DI 컨테이너 제공으로 OCP, DIP를 가능하게 지원해준다.
**클라이언트 코드의 변경 없이 기능 확장**

### 📕정리
모든 설계에 **역할**과 **구현**을 분리하자.
공연으로 예를 들면, 배역만 만들어 두고, 배우는 언제든지 유연하게 변경할 수 있도록 만드는 것이 좋은 **객체 지향 설계**이다.
이상적으로는 모든 설계에 인터페이스를 부여 하는것이다.

---

[인프런 스프링 핵심 원리 - 기본편](https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-%ED%95%B5%EC%8B%AC-%EC%9B%90%EB%A6%AC-%EA%B8%B0%EB%B3%B8%ED%8E%B8)
