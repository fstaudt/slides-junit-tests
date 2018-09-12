src/test/resources/application-test.yml
``` yaml
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

<span style="color:red">!! file 'src/test/resources/application.yml' cause failure in some IDE.</span>