# Use Java 17 Alpine JRE image
FROM eclipse-temurin:17-jre-alpine

# Set build-time argument for the JAR file location
ARG artifact=target/spring-boot-web.jar

# Set working directory inside the container
WORKDIR /opt/app

# Copy the Spring Boot JAR into the container
COPY ${artifact} app.jar

# Command to run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
