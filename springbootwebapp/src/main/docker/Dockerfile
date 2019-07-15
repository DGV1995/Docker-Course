FROM centos

RUN yum install -y java

VOLUME /tmp

# Name the application jar as 'myapp.jar'
ADD spring-boot-web-0.0.1-SNAPSHOT.jar myapp.jar

# Update the date of the jar file (important if we work with static resources such as images)
RUN sh -c "touch myapp.jar"

CMD ["java", "-jar", "myapp.jar"]

