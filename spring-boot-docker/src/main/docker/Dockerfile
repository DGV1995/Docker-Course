FROM openjdk:8-alpine

VOLUME /tmp

ADD maven/spring-boot-docker-0.0.1-SNAPSHOT.jar myapp.jar
RUN sh -c "touch myapp.jar"

CMD ["java", "-jar", "myapp.jar"]