### Unit tests vs integration tests
- integration tests (end-to-end) automated as JUnit tests are essential:
  - mandatory for cloud native applications
  - test of complete chain must be executed before commit
- relevance of unit tests must be challenged:
  - is it a duplicate of another test ?
  - does it make the production code more rigid ?
  - useless tests must be removed