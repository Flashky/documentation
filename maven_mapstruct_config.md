## Propiedades

En primer lugar, para que Eclipse funcione correctamente es necesario definir esta propiedad:
```xml
<properties>
	<!-- automatically run annotation processors within the incremental compilation -->
	<m2e.apt.activation>jdt_apt</m2e.apt.activation>
</properties>
```

## Dependencias
En dependencias, para Java 8 o superior:
```xml
<dependency>
    <groupId>org.mapstruct</groupId>
    <artifactId>mapstruct-jdk8</artifactId>
    <version>${org.mapstruct.version}</version> 
</dependency
```

Para versiones anteriores a Java 8
```xml
<dependency>
    <groupId>org.mapstruct</groupId>
    <artifactId>mapstruct</artifactId>
    <version>${org.mapstruct.version}</version> 
</dependency
```


## Plugins

Independientemente de artifactId usado para mapstruct, añadir lo siguiente:
```xml
<build>
  <plugins>
    <plugin>
        <groupId>org.apache.maven.plugins</groupId>
        <artifactId>maven-compiler-plugin</artifactId>
        <version>3.5.1</version>
        <configuration>
            <source>1.8</source>
            <target>1.8</target>
            <annotationProcessorPaths>
                <path>
                    <groupId>org.mapstruct</groupId>
                    <artifactId>mapstruct-processor</artifactId>
                    <version>${org.mapstruct.version}</version>
                </path>
            </annotationProcessorPaths>
        </configuration>
    </plugin>
  </plugins>
</build>
```
