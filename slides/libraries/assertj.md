### Assertj
- assertion library
- write highly readable assertions

``` java
import static org.assertj.core.api.Assertions.assertThat;

assertThat(account.getAccountId()).isEqualTo(TEST_ACCOUNT);
assertThat(account.getAmount()).isEqualTo(1);
```