# Use a suitable base image for your application
#FROM adoptopenjdk/openjdk11:alpine-jre
FROM adoptopenjdk:11-jre-hotspot
# Set the working directory inside the container
WORKDIR /app

# Copy the packaged JAR file into the container
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Specify the command to run on container startup
ENTRYPOINT ["java","-jar","/app.jar"]
