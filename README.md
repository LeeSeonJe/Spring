# Spring

## maven Setting
### maven 
- maven.apache.org
- download
  - ![image](https://user-images.githubusercontent.com/59919620/81405533-cd9ae080-9172-11ea-8097-dfccc3e826f9.png)
- Files
- Binary zip archive > Link
- apache-maven-3.6.3-bin.zip
  - ![image](https://user-images.githubusercontent.com/59919620/81405565-e0151a00-9172-11ea-9078-42d74b8d9650.png)

### apache-maven-3.6.3-bin.zip 압축풀기
- folder "repository" create
  - ![image](https://user-images.githubusercontent.com/59919620/81405615-fc18bb80-9172-11ea-86d5-47a35bccf53c.png)
- conf > settings.xml open
  - ![image](https://user-images.githubusercontent.com/59919620/81405708-28343c80-9173-11ea-8bd9-81f2c94f9bec.png)
- \<localRepository>/path/to/local/repo\</localRepository> 주석 밑으로 복사, 붙여넣기
- \<localRepository>"repository" localAddress 추가\</localRepository>
- ex) \<localRepository>E:\dev\apache-maven-3.6.3\repository\</localRepository>
  - ![image](https://user-images.githubusercontent.com/59919620/81405743-3aae7600-9173-11ea-8f90-aeba7d32c903.png)


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








# Spring 실행하기
### 1. STS Tool 사용하기
- spring.io 접속
- menu > project > Spring Tools4 
  - ![image](https://user-images.githubusercontent.com/59919620/81405371-75fc7500-9172-11ea-88de-f8ffa3857271.png)
- scroll을 쭉 내리다 보면 "Looking for Spring Tool Suite 3?" 부분에서 "Spring Tool Suite 3 wiki" click
  - ![image](https://user-images.githubusercontent.com/59919620/81405450-9cbaab80-9172-11ea-924d-b726b4c55f97.png)
- Spring Tool Suite 3.9.12 > full distribution on Eclipse @.@@ > 자신과 같은 Eclipse version 사용 / 버전이 달라도 괜찮음.
  - ![image](https://user-images.githubusercontent.com/59919620/81405485-b3f99900-9172-11ea-9cf7-9549f7ea05bd.png)
- download
- ex) **\"spring-tool-suite-3.9.12.RELEASE-e4.14.0-win32-x86_64.zip\"** 
- 압축을 해제 후 sts-bundle > sts-3.9.12.RELEASE > STS.exe 실행
  - ![image](https://user-images.githubusercontent.com/59919620/81405928-97119580-9173-11ea-94af-fd5f8b7c23e4.png)
- 실행하게 되면 이클립스처럼 실행되는걸 볼 수 있다.
  - ![image](https://user-images.githubusercontent.com/59919620/81406059-d809aa00-9173-11ea-8484-1ff8b5dc0b5a.png)


### 2. Eclipse Marketplace setup
- help > Eclipse Marketplace > "sts" search > Spring Tools 3 (Standalone Edition) @.@.@@.RELEASE install
  - ![image](https://user-images.githubusercontent.com/59919620/81406229-2a4acb00-9174-11ea-9073-ac614131957c.png)
  - ![image](https://user-images.githubusercontent.com/59919620/81406352-5e25f080-9174-11ea-9cab-2f1bf589973a.png)
  - ![image](https://user-images.githubusercontent.com/59919620/81406701-0b990400-9175-11ea-8705-ac7d82f5bf35.png)
  - ![image](https://user-images.githubusercontent.com/59919620/81406742-1eabd400-9175-11ea-84e6-e6f584d3e9bc.png)
- Restart Now가 나오면 Restart 해주자.
  - ![image](https://user-images.githubusercontent.com/59919620/81406778-2c615980-9175-11ea-8d18-da1e8d1d71c9.png)


# Spring project Create
