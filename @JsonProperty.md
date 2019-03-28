# Uson de @JsonProperty

**Sin @JsonProperty**

```java
public class Name {
  public String _first_name;
}
```

Resultado:
```json
{ "_first_name" : "Bob" }
```

**Con @JsonProperty**

```java
public class Name {
  @JsonProperty("firstName")
  public String _first_name;
}
```

Resultado:
```json
{ "firstName" : "Bob" }
```
