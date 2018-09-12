### Awaitility
- synchronize tests on asynchronous operations
- improved readability for tests with events

``` groovy
dependencies {
  testCompile('org.awaitility:awaitility:3.1.1')
}
```

``` java
import static org.awaitility.Awaitility.await;
import static java.util.concurrent.TimeUnit.SECONDS;

await().atMost(1, SECONDS).untilAsserted(
  () -> {
    assertThat(account.getBalance()).isEqualTo(1);
  }
);
```