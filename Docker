# Use an official OpenJDK runtime as a parent image
FROM openjdk:17-jdk-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the Spring Boot jar file from the local 'target' folder into the container
COPY target/Todoapp.jar /app/Todoapp.jar

# Expose port 8080 (default port for Spring Boot)
EXPOSE 8080

# Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "Todoapp.jar"]
