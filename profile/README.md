# Team Agile rules

### Versions

```
Java version: 8
Springboot version: 2.7.2
Denpency Versions: Demo code version
```

### Testing

```
Use JUnit with JACOCO
MockMVC for mvc controller testing
 - @WebMvcTest(EmployeeController.class)
 - @ExtendWith(MockitoExtension.class)
  
Mockito and H2 database for DAO and Service layers

Minimum coverage: 75%
Excluded application for coverage: Authentication Server, Email Service.

Core Service and Composite Service repositories includes Java for Maven Actions with github build/testing features.

```

### DB rules (For SQL scripts)

```
 - All databases name must start with capital letter.
   Following syllables must start with capital letter as well.

 - All table names must start with capital letter.
   Following syllables must start with capital letter as well. Most name should be noun.
 
 - Attribute names must be all lowercase. Follows snake-case (Example: "attribute_name").
   However, Java entity variables should be Camel case like "attributeName".

 - Must use databases based on each allocated user account to block usage confliction.

```


### Meeting time

```
August / 13 / 2022 (Friday) ~ 15 (Tuesday): EDT 7:00 P.M. 
16 (Wednesday) ~ 18 (Friday) : EDT 10 A.M.
```

### Team meeting contents:

1. Progress report
2. Suggestion
3. Discuss next story (with giving points)
4. Plan / Diagram fix
