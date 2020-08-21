# Sample Single Jar Spring Boot ReactJS App

Example combined single jar deployable demonstrating conccurrent front-end + back-end development workflow. 

![](https://github.com/vicsz/spring-boot-reactjs-single-jar/workflows/Build/badge.svg
)

SpringBoot (backend) and ReactJS (frontend) in single deployable jar file.

Java work is done out of the *java-app* directory. 

Note, the only build requirements are a Java JDK .. npm / node and gradle are all auto downloaded if needed. 

## To run the backend and frontend locally: 

```sh
./gradlew java-app:bootRun 
```

(default local address is localhost:8080)

## Frontend Development Workflow 

### Start the backend server (will be on localhost:8080)
```sh
./gradlew -a java-app:bootRun 
```
*Note the "-a" which skips building project dependencies .. in our case, the npm sub component.*

### Start the frontend server from the npm-app directory (will be on localhost:3000)

```sh
npm run start
```

*Note the proxy reference in the package.json that causes api calls to route to port 8080, and skip CORS checks*
