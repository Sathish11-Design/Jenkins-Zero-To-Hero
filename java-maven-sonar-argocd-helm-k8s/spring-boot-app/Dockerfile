# Use a lightweight JDK image instead of JRE
FROM eclipse-temurin:21-jdk-alpine

# Argument to specify the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# Copy the built JAR from target folder
COPY ${artifact} app.jar

# Run the application
ENTRYPOINT ["java","-jar","app.jar"]
