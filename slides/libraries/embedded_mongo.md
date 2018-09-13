### Embedded Mongo DB

- No external Mongo DB required for JUnit tests
- <span style="color:red">!!!</span> Workaround required to bypass Proxy 
- <span style="color:red">!!!</span> Mongo DB 4.0 not supported (yet)
- <span style="color:red">!!!</span> Not a Mongo DB official product

``` groovy
dependencies {
  testCompile('de.flapdoodle.embed:de.flapdoodle.embed.mongo')
}
```