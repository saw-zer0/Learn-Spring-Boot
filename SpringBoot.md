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

