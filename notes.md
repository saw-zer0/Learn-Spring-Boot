# Spring Boot notes

## Core concepts:
### IoC (Inversion of control):
- Design Principle
- Control of object creation and flow is inverted from the class itself to an external entity.

### DI (Dependency Injection): 
- Design pattern for loose coupling
- Instead of class creating its own dependencies, provided from outside
- Implementation of IoC
### IOC container : 
- Configure & manage Java Objects or **Spring Beans** - declared with @component, @service etc.
- Responsible for lifeCycle of Beans
- Uses Dependency injection (DI) to provide object reference during runtime
### AOP (Aspect Oriented Programming) ###
- Paradigm for modularity of cross-cutting concerns
- Cross-cutting concern - feature that affects multiple parts of system - eg. Logging, Security etc
- Works by creating proxy object at runtime
- Intercepts method calls and executes additional code

- __Parts of AOP__
    - **Aspect** - Cross-cutting concern logic
    - **Join Point** - specific execution point of method that is intercepted
    - **Advice** - action taken by aspect at a Join point - @After, @Before, @AfterThrowing etc.
    - **Pointcut** - expression that targets methods in a class / matches specific set of Join points - AspectJ pointcut expression language
    - **Target Object**/**Target Bean** - method with business logic
    - **AOP Proxy**/**Advised Bean** - A Wrapper around the target object - replace instance with proxy - intercepts method calls - generated at runtime
    - **Weaving** - The process of applying an aspect to target obejct at runtime - create *Advised Object*

    ![Example Aspect](ExampleAspect.png "Aspect Example")

    Here **userServiceMethods()** is an alias for pointcut expression - Named pointcut

### Data Access Framework (DAF) / Data Access Layer (DAL)
- High Level Architectural Concept
- Responsible for interaction with data sources
- Uses **Data Access Object(DAO)** pattern
    - Entity/Model
    - Repository/DAO
    - Service
    - Controller

## Project Setup
project starter -> start.spring.io

pom.xml -> Project Object Model -> Maven uses pom to download dependencies and build the project

src
- main
    - java - source code
        - java\com\tutorial\artifact - entry point 
    - resources - config, static files etc
        - application.properties - config file - do not sensitive info


Dependency management
- In order to build a web app following are needed:
    - tomcat - embedded server
    - web - handle web request
    - webmvc - building api
    - jackson - process JSON
    - logging 

    - In spring boot - spring-boot-starter-web

Maven Central:
- similar to www.npmjs.com for js packages
    - mvn install
    - vscode plugin maven for java

Spring MVC:
- Used to handle web request in spring boot
- annotations:
    - @controller
    - @RequestMapping()

Hot Reload:
- add spring-boot-devtools dependency to pom.xml

