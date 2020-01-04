# quarkus-gelf-include-full-mdc project

Small project to showcase a pull request on the main quarkus.io repository

# Usage

- Clone [the forked quarkus project](https://github.com/devauxbr/quarkus), checkout branch `feature/gelf-include-full-mdc` and build with `./mvnw clean install`
- Start Logstash locally by running `docker-compose up` in the root of this repository 
- In another terminal, start the project in dev mode with `./mvnw clean compile quarkus:dev` then make a request in another terminal with :
```
curl http://localhost:8080/greeting
```

You should see the field `"hello" => "mdc"` in the request log entry ! :tada:
