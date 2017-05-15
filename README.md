Reactive Apps
=============
This demo application showcases end-to-end `Functional Reactive Programming (FRP)` using the following technology stack:
* Spring Framework 5
* Spring Boot 2.0.0
* Spring WebFlux
* Embedded MongoDB
* Reactive MongoDB Driver

Highlights of this application are:
* Use of Server-Sent Events (SSE) rendered in HTML by Thymeleaf from a reactive data stream.
* Use of Server-Sent Events (SSE) rendered in JSON by Spring WebFlux from a reactive data stream. 
* Use of Spring Data MongoDB's reactive (Reactive Streams) driver support.
* Use of Spring Data MongoDB's support for infinite reactive data streams based on MongoDB tailable cursor (see [here](https://docs.mongodb.com/manual/core/tailable-cursors/)). 
* Use of Thymeleaf's fully-HTML5-compatible syntax.
* Use of `webjars` for client-side dependency managements.
* Reactive Netty as a server
* Multi-project builds with Gradle Kotlin Script. 
* Kotlin as a language
* Cross-Origin Resource Sharing (CORS)
* Docker deployment


### Running
> use `./gradlew` instead of `gradle` if you didn't installed `gradle`

Start all 3 apps: [mongo-data-service](./mongo-data-service), [stream-service](./stream-service), [ui-app](./stream-service)

### Testing
```bash
gradle test
```
### Building 
```bash
gradle build
```

### Gradle Commands
```bash
# upgrade project gradle version
gradle wrapper --gradle-version 3.5
# gradle daemon status 
gradle --status
gradle --stop
```


