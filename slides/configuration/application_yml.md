src/main/resources/application.yml
``` yaml
---
spring:
  profiles: test
test:
  config: value
```

``` java
@RunWith(SpringRunner.class)
@SpringBootTest(webEnvironment = SpringBootTest.WebEnvironment.RANDOM_PORT)
@ActiveProfiles("test")
public class ResourceTest {
}
```