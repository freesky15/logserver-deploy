FROM openjdk:20-jdk
RUN mkdir -p /app
RUN mkdir -p /app/logs
COPY logserver.jar /app/logserver.jar
WORKDIR /app
ENTRYPOINT ["java", "-jar", "logserver.jar"]
