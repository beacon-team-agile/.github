# Team Agile HR Management System

## Microservice architecture

 ![Micro Service relations](../img/Postman%20Execution%20-%20API%20call,%20reference%20diagram.png)

# Entity Relationship Diagram

<p align="center">
 <img src="../img/Postman%20Execution%20-%20Application%20ER%20diagram.png" width="550">
 </br>
 <img src="../img/Postman%20Execution%20-%20Authentication%20ER%20diagram.png" width="750">
 </br>
 <img src="../img/Postman%20Execution%20-%20Housing%20ER%20diagram.png" width="950">
</p>

# Postman Execution Examples

<img src="../img/Postman%20Execution%20-%20Postman%20Execution%20flow.png">

## Team Agile rules

### Versions

```
Java version: 8
Springboot version: 2.7.2. 
However, for mySQL DAO services, using 2.6.4 is permitted since 2.7+ does not handle null constraints on auto generated id.

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
   Otherwise this will create Criteria query request errors.
   
   Example: CREATE TABLE `Role`; not CREATE TABLE Role;
   
   FYI: You must include backquotes in Java Spring Entity to make a valid mapping.
   Example: @Column(name = "`User`") 
   
 - ALL sql-reserved commands are uppercase.
   
```

### github rules (For SQL scripts)

```
  - Branch names must be all lowercase with space replaced to '-'
  Ex) "firstname-repo-name"
```

### Spring Boot

```
   - Only application.properties files; no .yml file except for Eureka and Gateway applications
```

### REST API rules

```
   - url should all be lowercases
   - request header, body keys must be all lowercases
   - all space must be replaced by '-'
   - Mostly use verbs
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


