# Use a suitable base image for your application (arm64 architecture)
#FROM arm64v8/openjdk:11-jre-slim
FROM arm64v8/openjdk:11-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the packaged JAR file into the container
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Specify the command to run on container startup
ENTRYPOINT ["java","-jar","/app.jar"]
