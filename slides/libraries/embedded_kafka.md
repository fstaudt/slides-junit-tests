### Embedded Kafka

- No external Kafka required for JUnit tests
- <span style="color:red">!! integration with AVRO schema registry to investigate</span>

``` groovy
dependencies {
  testCompile ('org.springframework.kafka:spring-kafka-test')
}
```
``` yaml
spring:
  profiles: test
  kafka:
    bootstrap-servers: ${spring.embedded.kafka.brokers}
```

``` java
public class ResourceTest {
    @ClassRule
    public static KafkaEmbedded kafka = new KafkaEmbedded(1, true, "test");
}
```