# Uso de @JsonFormat

**Fecha con formato ISO-8601**

```java
public MyDate {
  @JsonFormat(shape = JsonFormat.Shape.STRING, pattern = "yyyy-MM-dd")
  private Date myDate;
}
```

Resultado:

```json
{ "myDate": "2019-03-28" }
```

**Fecha cómo número de segundos desde epoch**

```java
public MyDate {
  @JsonFormat(shape = JsonFormat.Shape.NUMBER)
  private Date myDate;
}
```

Resultado:

```json
{ "myDate": 1482054723876 }
```
