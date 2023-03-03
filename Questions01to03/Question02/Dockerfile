# First stage: Build the application
FROM maven:3.6.3-jdk-11 AS build
COPY ./spring-boot-maven-example-helloworld /app
WORKDIR /app
RUN mvn clean package

# Second stage: Run the application
FROM openjdk:11-jre-slim
COPY --from=build /app/target/SpringBootMavenExample-1.3.5.RELEASE.jar /app/app.jar
EXPOSE 9095
CMD ["java", "-jar", "/app/app.jar"]