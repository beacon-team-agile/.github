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
   Camel case.

 - All table names must start with capital letter.
   Following syllables must start with capital letter as well. Most name should be noun as possible.
   Camel case.
 
 - Attribute names must be all lowercase. Follows snake-case (Example: "attribute_name").
   However, Java entity variables should be Camel case like "attributeName".

 - Must use databases based on each allocated user account to block usage confliction.
 
 - Any naming those are reserved as RDS/MySQL keywords has to be labeled with back quotes (`)
   Example: CREATE TABLE `Role`; not CREATE TABLE Role;
   
   FYI: You must include backquotes in Java Spring Entity to make a valid mapping.
   Example: @Column(name = "`User`") 
```

### github rules (For SQL scripts)

```
  - Branch names must be all lowercase with space replaced to '-'
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
