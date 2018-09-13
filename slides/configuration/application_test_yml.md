### separate file 'application-test.yml'
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

<span style="color:red">!!!</span> don't duplicate file 'application.yml' in 'src/test/resources':
  - not correctly handled by some IDE (Eclipse)
  - need for duplicate configuration