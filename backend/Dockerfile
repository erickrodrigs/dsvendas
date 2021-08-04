FROM maven:3.6.0-jdk-11-slim AS build

ENV PORT=8080

WORKDIR /usr/src/app

COPY ./src ./src

COPY ./pom.xml .

RUN mvn -f pom.xml clean package -DskipTests

FROM adoptopenjdk/openjdk11:jre11u-alpine-nightly

COPY --from=build /usr/src/app/target/dsvendas-0.0.1-SNAPSHOT.jar app.jar

EXPOSE ${PORT}

CMD ["java", "-jar", "app.jar"]
