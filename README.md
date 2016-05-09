# Mule Microservice

The example shows how to create a runnable Jar file with Mule Embedded.

The example uses Mule CE 3.7.0, but it works perfectly with Mule EE (for Mule EE you need Mule License), to run with Mule EE you need to incluede the license file in src/main/resources.

##Requirements

a) Java 7+

b) Gradle 2.10+

## How to run it

1) Clone the project

2) Go in the directory

3) Execute 

```
gradle clean microserviceJar
```

4) Run
 
```
java -jar build/libs/mule-example-1.0-microservice.jar 
```

5) Go to http://localhost:8081/mule-ms

You should see in you browser: "Hello World from Mule Microservice"