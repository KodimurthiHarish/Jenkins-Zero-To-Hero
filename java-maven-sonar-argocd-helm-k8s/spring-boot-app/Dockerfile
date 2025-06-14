# Base image with Java 17 (alpine version for smaller size)
FROM adoptopenjdk/openjdk17:alpine-jre

# Use the JAR built from Maven (keep your artifact name the same)
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the jar to container with the same name
COPY ${artifact} app.jar

# Entry point for running the Spring Boot app
ENTRYPOINT ["java", "-jar", "app.jar"]
