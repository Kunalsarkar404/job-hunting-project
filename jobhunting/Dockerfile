# Use an official OpenJDK runtime as a parent image
FROM openjdk:17-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the jar file from the target directory into the container
COPY target/jobhunting-0.0.1-SNAPSHOT.jar /app/jobhunting.jar

# Expose the port the app will run on
EXPOSE 8081

# Run the Spring Boot app
ENTRYPOINT ["java", "-jar", "/app/jobhunting.jar"]
