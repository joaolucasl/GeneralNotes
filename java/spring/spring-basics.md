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


