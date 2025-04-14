# Use a more recent base image with OpenJDK 17 (better security)
FROM openjdk:8u151-jdk-alpine3.7

# Expose the application port
EXPOSE 8070

# Set the app home directory
ENV APP_HOME=/usr/src/app  

# Copy the jar file from target folder into the Docker image
COPY target/app.jar $APP_HOME/app.jar

# Set the working directory
WORKDIR $APP_HOME

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
