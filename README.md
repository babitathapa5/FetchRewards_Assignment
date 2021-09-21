# FetchRewards_Assignment
Babita, Backend, Take Home Test from Fetch Reward

## Requirements

For building and running the application you need:

- [JDK 1.8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
- [Maven 3](https://maven.apache.org)

## Running the application locally

There are several ways to run a Spring Boot application on your local machine. One way is to execute the `main` method in the `de.codecentric.springbootsample.Application` class from your IDE.

Alternatively you can use the [Spring Boot Maven plugin](https://docs.spring.io/spring-boot/docs/current/reference/html/build-tool-plugins-maven-plugin.html) like so:

```shell
mvn spring-boot:run
```

## Consumption Guide
Resources Available:
```shell
● Adding transactions for a specific payer and date.
  METHOD : POST
  PATH : /api/transaction
  SAMPLE INPUT BODY (JSON): { "payer": "MILLER COORS", "points": 10000, "timestamp": "2020-11-01T14:00:00Z" }
  SAMPLE OUTPUT RESPONSE (JSON) : 
  ```shell
  Transaction Updated Sucessfully
  
```
 
```shell
● Spending points using the rules above and return a list of { "payer": <string>, "points": <integer> } for each call.
  METHOD : POST
  PATH : /api/points
  SAMPLE INPUT BODY(JSON):```shell { "points": 100 }```
  SAMPLE OUTPUT RESPONSE (JSON) : 
  {
    "MILLER COORS": -100
  }
```
  
```shell
● Returning all payer point balances.
  METHOD : GET
  PATH : /api/balance
  ```shell
  SAMPLE OUTPUT RESPONSE (JSON) : 
  {
    "MILLER COORS": 9900
  }
 ```
  
