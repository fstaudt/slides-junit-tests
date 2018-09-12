### Avoid external dependencies
- external dependencies should be avoided to ease onboarding of developers:
  - DB started with JUnit tests (embedded mongoDB, H2)
  - Kafka broker started with unit tests (embedded Kafka)
  - Wiremock server to mock microservice interactions

- external dependencies should be documented in README otherwise