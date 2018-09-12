### Embedded Mongo DB

- No external Mongo DB required for JUnit tests
- <span style="color:red">!! Workaround required to bypass Proxy</span> 
- <span style="color:red">!! Mongo DB 4.0 not supported (yet)</span>
- <span style="color:red">!! Not a Mongo DB official product</span>

``` groovy
dependencies {
  testCompile('de.flapdoodle.embed:de.flapdoodle.embed.mongo')
}
```