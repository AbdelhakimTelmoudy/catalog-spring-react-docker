# Use a slim Java base image
FROM openjdk:17-slim

# Set working directory for the application
WORKDIR /app

# Create a directory for the application JAR
RUN mkdir app

# Copy the application JAR
COPY target/*.jar app/app.jar

# Expose the port your application listens on (replace 8080 with your actual port)
EXPOSE 8080

# Set environment variables (if needed)
ENV APP_ENV=production

# Define the command to run the application
ENTRYPOINT ["java", "-jar", "app/app.jar"]
