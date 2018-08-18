---
name: Request Help issue template
about: Describe Request Help

---

# Q. `<Issue Title>`

> FIXME: Describe the task in free format
> 육하원칙에 따른 자세한 설명일수록 좋다
* `<something task description>`


## Issue
```
FIXME: fill source code or log
...
```

## Expected Result
> FIXME: Describe the expected result
* `<something>`

<br>

## Actual Result
> FIXME: Describe the actual result
* `<something>`

<br> 

## relate to issue
> FIXME: Describe relate to issue
* `<issue title> <#issue number>`

<br>

> #### Reference
> FIXME: fill reference link
> * `[title](link)`

---

<br>

> FIXME: Remove below example content
# Example

# Q. JPA에서 단건 조회가 왜 안되나요?

## Issue
* [JPA / Hibernate One to Many Mapping Example with Spring Boot](https://www.callicoder.com/hibernate-spring-boot-jpa-one-to-many-mapping-example/)를 보고 mapping한 후 단건 조회를 했는데 아래와 같은 문제가 발생합니다
* commit: #56fd24
```java
java.lang.RuntimeException: Unable to instantiate application com.example.test
at java.lang.reflect.Method.invokeNative(Method.java)
at java.lang.reflect.Method.invoke(Method.java:515)
...

public class Product {

    @Id
    private Long productId;

    @ManyToOne
    private User user;
    ...
}
```

<br>

## Expected Result
* 상품 ID로 단건의 상품을 조회하고 싶어요

<br>

## Actual Result
* 아래 stacktrace의 RuntimeException 발생
```java
java.lang.RuntimeException: Unable to instantiate application com.example.test
at java.lang.reflect.Method.invokeNative(Method.java)
at java.lang.reflect.Method.invoke(Method.java:515)
...
```

<br>

## relate to issue
* 상품 단건 조회 API 구현 #15

<br>

> #### Reference
> [JPA / Hibernate One to Many Mapping Example with Spring Boot](https://www.callicoder.com/hibernate-spring-boot-jpa-one-to-many-mapping-example/)
