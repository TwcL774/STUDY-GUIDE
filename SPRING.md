# Spring

## What is Spring

* Spring is an open-source application framework and inversion of control container for the Java platform. It provides a lightweight container for managing Java objects and their dependencies, making it easier to write Java applications that are easy to test, maintain, and extend.

* Spring is organized around a set of modules, each of which provides a specific set of functionality. Some of the main modules in Spring include:

    - Core: Provides the fundamental parts of the Spring framework, including the IoC container, dependency injection, and resource management.

    - Data Access: Provides support for working with data access technologies such as JDBC, Hibernate, and JPA.

    - Web: Provides support for building web applications, including MVC frameworks and web sockets.

    - AOP: Provides support for aspect-oriented programming, allowing developers to define reusable cross-cutting concerns such as logging and transaction management.

    - Security: Provides support for security in web applications, including authentication and authorization.

* Spring is often used in enterprise Java applications to provide a consistent, flexible, and easy-to-use foundation for building applications. It is also widely used in web applications and microservices, and can be easily integrated with other frameworks and technologies such as Hibernate, JPA, and Maven.

* Inversion of control (IoC) is a software design principle in which the flow of control of a system is inverted in comparison to traditional control flow. In a traditional program, the control flow is determined by the program itself. In an IoC system, the control flow is determined by an external entity, often referred to as an "IoC container."

* There are two main types of IoC: dependency injection (DI) and service locator.

    - In dependency injection, objects are given their dependencies (objects they need to function) at creation time through a constructor, method, or field. This allows for more flexibility and makes it easier to test and maintain the code, as the dependencies can be easily swapped out or mocked.

    - In service locator, objects are responsible for finding their own dependencies, often through a central registry. This can be less flexible and more difficult to test and maintain, as the dependencies are not explicitly passed to the object.

* IoC is a useful design principle as it allows for more flexibility and modularity in a system. It can make it easier to test and maintain code, as dependencies can be easily swapped out or mocked. It also promotes the separation of concerns, as objects are not responsible for creating or finding their own dependencies.

* An opinionated framework is a software framework that provides a set of standardized and often rigid guidelines for developing applications within a specific domain. It typically comes with a set of pre-defined conventions and a set of tools that are designed to enforce these conventions. It may also come with a set of default configurations and settings that are intended to promote best practices and encourage developers to adhere to a certain set of guidelines.

## Spring Boot

* Spring Boot is a Java-based framework that provides a simple and easy-to-use approach for creating stand-alone, production-grade Spring-based applications. It takes an opinionated view of the Spring platform, meaning that it comes with a set of default configurations and dependencies that are suitable for most applications.

* One of the main goals of Spring Boot is to make it easy to create Spring-based applications that can be "just run." This means that it includes an embedded Tomcat server, so you don't have to worry about installing and configuring a separate web server. It also includes a number of other features to make it easy to create and run a Spring application, including:

    - Automatic configuration: Spring Boot can automatically configure your application based on the dependencies that you have added. For example, if you add the spring-webmvc dependency, Spring Boot will automatically configure a DispatcherServlet and other necessary components for a web application.

    - Starter dependencies: Spring Boot provides a number of "starter" dependencies that allow you to easily add the necessary dependencies for a particular type of application. For example, the spring-boot-starter-web dependency includes the dependencies for a web application, including spring-webmvc and tomcat-embed-jasper.

    - Command-line interface: Spring Boot includes a command-line interface (CLI) that you can use to quickly create and run Spring applications.

    - Actuator: Spring Boot includes a number of "actuator" endpoints that provide useful information about your application, such as the current health of the application, the number of requests being handled, and the amount of memory being used.

Spring Boot is a useful tool for quickly creating and deploying Spring-based applications. It makes it easy to get started and eliminates much of the setup and configuration that is required for a typical Spring application.

### Spring Web

* Spring Web is a module in the Spring Framework that provides support for building web applications, including web services, web resources, and web user interfaces. It is built on top of the Spring Core module and provides a number of features for developing web applications, including:

    - Spring MVC: A Model-View-Controller (MVC) framework for building web applications. It provides support for handling HTTP requests, mapping request data to objects, and rendering views using templates.

    - Spring WebFlux: A reactive web framework that is built on top of the Reactor project. It allows developers to build non-blocking, asynchronous web applications that can scale to handle a large number of concurrent requests.

    - mSpring Web Services: A framework for building web services using the Simple Object Access Protocol (SOAP) and the Representational State Transfer (REST) architectural styles. It provides support for building both client and server-side web services.

    - Spring Web Socket: A framework for building web applications that use the WebSocket protocol for bi-directional communication between the client and server.

* Spring Web is a useful tool for building web applications in the Java ecosystem. It provides a number of features for handling HTTP requests, building web services, and building reactive web applications. It is built on top of the Spring Core module and can be easily integrated with other Spring modules such as Spring Data and Spring Security.

### Spring Data

* Spring Data is a module in the Spring Framework that provides support for working with data access technologies such as JDBC, Hibernate, and JPA. It is designed to make it easier to build applications that need to work with data stored in a variety of databases and data stores.

* Spring Data provides a number of features for working with data, including:

    - Repository support: Spring Data provides a repository abstraction that allows you to create repositories for specific types of entities. These repositories provide a number of common CRUD (create, read, update, delete) operations, as well as support for pagination and sorting.

    - Query generation: Spring Data provides support for generating queries based on method names. This allows you to write queries using a simple method name convention, rather than having to write out the entire query using JPQL or SQL.

    - Transaction management: Spring Data provides support for managing transactions when working with data. It can automatically handle the transaction demarcation for you, making it easier to work with data in a transactional manner.

    - Integration with other Spring modules: Spring Data integrates with other Spring modules such as Spring MVC and Spring Security, making it easy to use in web applications and microservices.

* Spring Data is a useful tool for building applications that need to work with data stored in a variety of databases and data stores. It provides a number of features for working with data, including repository support, query generation, and transaction management, and can be easily integrated with other Spring modules.

### Spring Actuator

* Spring Actuator is a module in the Spring Framework that provides production-ready features for monitoring and managing Spring-based applications. It provides a number of "actuator" endpoints that allow you to monitor and manage your application in production.

* Some of the main features provided by Spring Actuator include:

    - Health: Actuator provides an endpoint that allows you to check the health of your application. This can be useful for monitoring and alerting purposes, as well as for load balancers that need to determine if an application is healthy before routing traffic to it.

    - Metrics: Actuator provides a number of metrics that can be useful for monitoring and debugging your application in production. These metrics include things like the number of requests being handled, the amount of memory being used, and the number of threads being used.

    - Logging: Actuator provides an endpoint that allows you to view the log files of your application. This can be useful for debugging and troubleshooting issues in production.

    - Auditing: Actuator provides support for auditing events in your application. This can be useful for tracking changes made to your application in production.

* Spring Actuator is a useful tool for monitoring and managing Spring-based applications in production. It provides a number of endpoints that allow you to check the health of your application, view metrics and logs, and audit events in your application.


# VS Code
[x] Install Spring Boot Extension Pack
[x] CTRL+SHIFT+P then type Spring Initializr: Create Maven Project
[x] add Spring Web
[x] add Spring DATA -JPA
[x] add Actuator
[x] add PostgreSQL
[x] add lombok
