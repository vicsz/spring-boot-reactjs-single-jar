# Sample Single Jar Spring Boot ReactJS App

![](https://github.com/vicsz/spring-boot-reactjs-single-jar/workflows/Build/badge.svg
)

SpringBoot (backend) and ReactJS (frontend) in single deployable jar file.

Java work is done out of the *java-app* directory. 

# To run the backend and frontend locally: 

```sh
./gradlew java-app:bootRun 
```

(default local address is localhost:8080)

# For development of ReactJS work out of the *npm-app* directory

Npm commands can be run traditionally (via npm directly) or via Gradle (i.e. gradle npm_start, gradle npm_run, etc)

Out of the *npm-app* directory, the default local address is localhost:3000.
