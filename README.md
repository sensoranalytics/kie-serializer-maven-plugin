# maven-kie-serializer-plugin
Kie serializer for Maven that really works

## Example

```xml
<plugin>
  <groupId>com.savi.maven.plugins</groupId>
  <artifactId>kie-serializer-maven-plugin</artifactId>
  <version>1.0.0</version>
  <extensions>true</extensions>
  <configuration>
    <!-- resDirectory is where the resulting serialized file lands -->
    <resDirectory>${project.basedir}/target/classes</resDirectory>
    <!-- The KieBase to serialize, as configured in kmodule.xml -->
    <kiebases>ShipmentKBase</kiebases>
  </configuration>
  <executions>
    <execution>
      <phase>compile</phase>
      <goals>
        <goal>serialize</goal>
      </goals>
    </execution>
  </executions>
</plugin>
```
