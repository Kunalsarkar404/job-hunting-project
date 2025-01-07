# Use a base image with Java and Maven
FROM maven:3.8.4-openjdk-17 AS build

# Set the working directory inside the container
WORKDIR /app

# Copy the pom.xml and install dependencies
COPY pom.xml .
RUN mvn dependency:go-offline

# Copy the source code and build the application
COPY src ./src
RUN mvn clean package -DskipTests


# Create the final image using a lighter Java runtime base image
FROM openjdk:17-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the JAR file from the builder image
COPY --from=build /app/target/jobhunting-0.0.1-SNAPSHOT.jar .

# Expose the application port
EXPOSE 8080

# Run the application
CMD ["java", "-jar", "/app/jobhunting-0.0.1-SNAPSHOT.jar"]
