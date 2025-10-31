# Spring Boot Notes 

## What is Spring Boot?
- Built on top of Spring framework
- Automatically Configures therefore no need for manual config
### Starter files:
- Pom or Gradle
- Facilitate Auto Config
- Add required Dependencies

## Why Spring Boot?
- Standalone Apps
- Embeded servers
- Comes with Maven or Gradle (Opiniated Starters)
- Auto Configures Spring Framework
- Production Ready Features - Health Checks, Metrics, Externalized Configs

##  Project Setup
project starter -> start.spring.io

## Files and Folders
- pom.xml -> **Project Object Model** -> Maven uses pom to download dependencies and build the project
- .mvn -> contains mvn wrapper properties|JAR etc for maven wrapper extension
- src
    - main
        - java - source code
            - java\com\tutorial\artifact - entry point 
        - resources - config, static files etc
            - **application.properties** - config file - do not put sensitive info
- mvnw | mvnw.cmd -> maven wrapper scripts 

## Dependency management
- In order to build a web app following are needed:
    - tomcat - embedded server
    - web - handle web request
    - webmvc - building api
    - jackson - process JSON
    - logging 

    - In spring boot - spring-boot-starter-web

## Maven Central:
- similar to www.npmjs.com for js packages
    - mvn install
    - vscode plugin maven for java

## Spring Boot Annotations:
@SpringBootApplication

## Quick Tips
Hot Reload:
- add spring-boot-devtools dependency to pom.xml
---
# How does Spring Boot Application Start?
## Spring Application Startup Process
**Before the `main()` function:**

1.  `JVM` initializes, loads the `main` class.
2.  `Static` initializers run in `sequence`.

**Inside `SpringApplication.run()`:**

3.  `SpringApplication` instance created; detects `web` type.
4.  `Run` listeners activated; `starting event` published.
5.  `Environment` configured from properties, YML, system `variables`.
6.  `EnvironmentPreparedEvent` is published to listeners.
7.  `ApplicationContext` `type` determined and `created`.
8.  `Initializers` executed on the `context` instance.
9.  `ApplicationPreparedEvent` is published to listeners.
10. `Context` refreshes; main `bean creation` phase.
11. `Bean definitions` loaded via `component scan`.
12. `Auto-configuration` activates based on `classpath` contents.
13. `Bean factories` post-processed for `modifications`.
14. `Bean post-processors` register for later `use`.
15. `Singletons` instantiated, wired via `dependency injection`.
16. `Lifecycle` callbacks like `@PostConstruct` are called.
17. `AOP` proxies applied for specific `features`.
18. `ContextRefreshedEvent` and `StartedEvent` published.
19. `Embedded server` starts listening for requests.
20. `CommandLineRunner` or `ApplicationRunner` execute their logic.
21. `ApplicationReadyEvent` published; application fully operational.