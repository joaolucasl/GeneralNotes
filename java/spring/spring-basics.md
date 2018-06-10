# Spring Framework

- *beans*: A bean is what an instance of a class is called in Spring;
- *ApplicationContext*: It stores the environmental information about the application;
  - Beans can be configured with XML or Annotations and loaded into the application context

## Inversion Of Control
A way to give components their dependencies and to manage them in the life cycle.

### Dependency Injection
- *Lookup*: When the code itself looks up for its own dependency. E.g.:
  ```
  context.getBean("payments_stream", PaymentsStream.class);
  ```

- *Injection*: When the code defines its dependencies either in its constructor or in its getters and setters.

#### Component Scan
- *Spring Boot*: 
    - If your other packages hierarchies are below your main app with the `@SpringBootApplication` annotation, you’re covered by implicit components scan.
    - If there are beans/components in other packages which are not sub packages of the main package, you should manually add them as `@ComponentScan`:
    ```
    @ComponentScan("com.github.joaolucasl.foo")
    @SpringBootApplication
    public class SpringApplication {
    ```
