FROM maven:3.6.0-jdk-11-slim AS build
WORKDIR /app
COPY . /app
# RUN mvn clean install
# ARG JAR_FILE=target/*.jar
COPY target/*.jar app.jar
ENTRYPOINT ["java","-jar","app.jar"]
EXPOSE 8080