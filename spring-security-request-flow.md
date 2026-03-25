# Spring Security Request Flow

## Core Architecture

### DelegatingFilterProxy

-   Lives in Servlet Container
-   Acts as a bridge between web server and Spring ApplicationContext

### FilterChainProxy

-   Lives in Spring Context
-   Central entry point for security logic
-   Chooses which SecurityFilterChain to apply

### SecurityFilterChain

-   Defines URL pattern (example: /api/\*\*)
-   Contains list of filters

### Security Filters

-   Perform actual work
-   Example:
    -   Authentication
    -   Authorization
    -   CSRF protection

------------------------------------------------------------------------

## Request Flow

Example request: `/api/orders`

1.  Request hits servlet container (like Tomcat)
2.  DelegatingFilterProxy intercepts request
3.  It forwards request to FilterChainProxy
4.  FilterChainProxy selects matching SecurityFilterChain
5.  Request passes through multiple security filters:
    -   Authentication filter
    -   Authorization filter
    -   CSRF filter
6.  If all checks pass → request reaches controller
7.  Response goes back through filter chain

------------------------------------------------------------------------

## Notes

-   Filters execute in defined order
-   If any filter fails → request is blocked
-   Spring Security is filter-based architecture
