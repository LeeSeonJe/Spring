# Spring

## maven Setting
### maven 
- maven.apache.org
- download
- Files
- Binary zip archive > Link
- apache-maven-3.6.3-bin.zip

### apache-maven-3.6.3-bin.zip 압축풀기
- folder "repository" create
- conf > settings.xml open
- \<localRepository>/path/to/local/repo\</localRepository> 주석 밑으로 복사, 붙여넣기
- \<localRepository>"repository" localAddress 추가\</localRepository>
- ex) \<localRepository>E:\dev\apache-maven-3.6.3\repository\</localRepository>


## Spring Study
### Spring Framework
#### - 자바 플랫폼을 위한 오픈 소스 애플리케이션 프레임워크 (자바 프레임워크) 간단하게 스프링(Spring)이라고 부름
- 특징
  - DI(Dependency Injection) 의존성 주입
    - **설정 파일**이나 **어노테이션**을 통해 **객체 간의 의존 관계**를 설정하여 개발자가 직접 의존하는 객체를 생성할 필요 없음
  - Spring AOP 관점 지향 프로그래밍
    - **트랜잭션**, **로깅**, **보안** 등 여러 모듈, 여러 계층에서 공통으로 필요로 하는 기능의 경우 해당 기능들을 분리하여 관리
    - 공통적으로 관리해야하는 부분들을 가져와 필요한 시점에 따라 코드를 보내준다.
  - POJO(Plain Old Java Object) 
    - 일반적인 J2EE 프레임워크에 비해 특정 라이브러리를 사용할 필요가 없어 개발이 쉬우며 기존 라이브러리의 지원 용이
  - IoC(Inversion of Control) 제어반전
    - **컨트롤의 제어권**이 개발자가 아니라 **프레임워크**에 있다는 뜻
    - **객채의 생성**부터 **모든 생명주기의 관리**까지 프레임워크가 주도
    - 객체를 생성하고 직접 호출하는 프로그램이 아니라 만들어둔 자원을 호출하여 사용
    
  - Spring JDBC 
    - MyBatis나 Hibernate 등의 데이터베이스를 처리하는 영속성 프레임워크와 연결할 수 있는 인터페이스 제공
  - Spring MVC
    - MVC 디자인 패턴을 통해 웹 애플리케이션의 Model, View, Controller 사이의 의존 관계를 DI 컨테이너에서 개발자가 아닌 서버가 객체들을 관리하는 웹 애플리케이션 구축
  - PAS(Portable Service Abstraction)
    
    
### Spring의 구성 모듈
- Data 접근 계층
- MVC 계층
- AOP 계층
- Core Container
  - Spring의 핵심 부분
  - Spring의 근간이 되는 **IoC**(또는 **DI**) 기능을 지원하는 영역담당
  - **BeanFactory**를 기반으로 **Bean**클래스들을 제어할 수 있는 기능 지원
  
  
  
### Spring 동작 구조
- Spring 애플리케이션
- Spring 웹
