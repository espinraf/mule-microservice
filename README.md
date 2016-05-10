# Mule Microservice

The example shows how to create a runnable Jar file with Mule Embedded.

The example uses Mule CE 3.7.0, but it works perfectly with Mule EE (for Mule EE you need Mule EE License).  

For Mule EE, you need:

+ Include Mule EE license file in src/main/resources.

+ In build.gradle file add user/password for Mule EE repository,
update the muleEnterprise flag to true and update muleversion to the desired Mule EE version  (see https://github.com/mulesoft-labs/mule-gradle-plugin).

```
mule.version = '3.7.3'
mule.muleEnterprise = true
mule.enterpriseRepoUsername = 'your-username'
mule.enterpriseRepoPassword = 'your-password'
```

The Gradle build file uses the the following plugins to create the jar file:

+ Mule Gradle Plugin https://github.com/mulesoft-labs/mule-gradle-plugin

+ Casule Gradle Plugin https://github.com/danthegoodman/gradle-capsule-plugin

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

Contact:
Rafael Espino (rafael.espino@redpill-linpro.com)

