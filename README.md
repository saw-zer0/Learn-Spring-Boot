
# Learn Spring with Quick notes

This workspace contains notes on Spring Framework and Spring Boot.

- [Spring Framework](./SpringFramework.md) Notes for core concepts of Spring, dependency injection, AOP etc.
- [Spring Boot](./SpringBoot.md) Notes about Spring Boot starters, project setup, auto-configuration, and the application startup process.

Images used by the notes are stored in `images/` (relative to this `notes/` folder).

Open either file to get started with the notes.
## Table of contents

### Spring Framework

- [Core concepts](./SpringFramework.md#core-concepts)
  - [IoC (Inversion of control)](./SpringFramework.md#ioc-inversion-of-control)
  - [DI (Dependency Injection)](./SpringFramework.md#di-dependency-injection)
  - [Spring Bean](./SpringFramework.md#spring-bean)
    - [Life cycle of a Bean](./SpringFramework.md#life-cycle-of-a-bean)
  - [IOC container](./SpringFramework.md#ioc-container)
    - [Configuring Spring Beans](./SpringFramework.md#configuring-spring-beans)
      - [Using Java Code](./SpringFramework.md#using-java-code)
  - [Sub-types of Spring Components](./SpringFramework.md#sub-types-of-spring-components)
  - [Bean Naming](./SpringFramework.md#bean-naming)
  - [Types of Dependency Injection](./SpringFramework.md#types-of-dependency-injection)
    - [Constructor Injection](./SpringFramework.md#constructor-injection)
    - [Field Injection](./SpringFramework.md#field-injection)
    - [Method Injection (Used in Configuration Methods)](./SpringFramework.md#method-injection-used-in-configuration-methods)
    - [Setter Methods Injection](./SpringFramework.md#setter-methods-injection)
  - [Mechanism for Dependency Resolution](./SpringFramework.md#mechanism-for-dependency-resolution)
    - [Type injection](./SpringFramework.md#type-injection)
    - [Named injection](./SpringFramework.md#named-injection)
  - [Bean Scope](./SpringFramework.md#bean-scope)
    - [Define Bean Scope in code](./SpringFramework.md#define-bean-scope-in-code)
    - [Types of Bean Scoping provided by Spring](./SpringFramework.md#types-of-bean-scoping-provided-by-spring)
  - [Special Spring Bean](./SpringFramework.md#special-spring-bean)
    - [Bean Environment](./SpringFramework.md#bean-environment)
    - [Bean Profile](./SpringFramework.md#bean-profile)
      - [@Profile to control which bean is loaded](./SpringFramework.md#profile-to-control-which-bean-is-loaded)
      - [Programmatical profile Activation](./SpringFramework.md#programmatical-profile-activation)
      - [Activated by spring.profiles.active](./SpringFramework.md#activated-by-spring-profiles-active)
  - [@Value Annotation](./SpringFramework.md#value-annotation)
    - [Example](./SpringFramework.md#example)
    - [Dynamic Expression to resolve Beans](./SpringFramework.md#dynamic-expression-to-resolve-beans)
  - [@PropertySource](./SpringFramework.md#propertysource)
    - [@PropertySources](./SpringFramework.md#propertysources)
  - [AOP (Aspect Oriented Programming)](./SpringFramework.md#aop-aspect-oriented-programming)
    - [Parts of AOP](./SpringFramework.md#parts-of-aop)
  - [Data Access Framework (DAF) / Data Access Layer (DAL)](./SpringFramework.md#data-access-framework-daf-data-access-layer-dal)
  - [MVC](./SpringFramework.md#mvc)
    - [MVC Annotations](./SpringFramework.md#mvc-annotations)
    - [Data types](./SpringFramework.md#data-types)
  - [Spring Data JPA (Model layer)](./SpringFramework.md#spring-data-jpa-model-layer)
    - [JPA Annotations](./SpringFramework.md#jpa-annotations)
  - [Service Layer](./SpringFramework.md#service-layer)
  - [Data Validation](./SpringFramework.md#data-validation)
  - [Error Handling](./SpringFramework.md#error-handling)
  - [Testing](./SpringFramework.md#testing)
    - [Annotations](./SpringFramework.md#annotations)
    - [Unit Testing](./SpringFramework.md#unit-testing)
    - [Integration Testing](./SpringFramework.md#integration-testing)
    - [Test Isolation](./SpringFramework.md#test-isolation)
      - [Mockito](./SpringFramework.md#mockito)
  - [Best Practices in Spring](./SpringFramework.md#best-practices-in-spring)
  - [Spring Rest](./SpringFramework.md#spring-rest)

### Spring Boot

- [What is Spring Boot?](./SpringBoot.md#what-is-spring-boot)
  - [Starter files](./SpringBoot.md#starter-files)
- [Why Spring Boot?](./SpringBoot.md#why-spring-boot)
- [Project Setup](./SpringBoot.md#project-setup)
- [Files and Folders](./SpringBoot.md#files-and-folders)
- [Dependency management](./SpringBoot.md#dependency-management)
- [Maven Central](./SpringBoot.md#maven-central)
- [Spring Boot Annotations](./SpringBoot.md#spring-boot-annotations)
- [Quick Tips](./SpringBoot.md#quick-tips)
- [Spring Application Startup Process](./SpringBoot.md#spring-application-startup-process)


