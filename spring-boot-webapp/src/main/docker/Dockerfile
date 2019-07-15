#FROM centos

#RUN yum install -y java

FROM openjdk:8-alpine

ENV LANG C.UTF-8

ENV JAVA_HOME /usr/local/openjdk-8
ENV PATH $JAVA_HOME/bin:$PATH

VOLUME /tmp

# Add the executable jar and name it as 'myapp.jar'
ADD spring-boot-web-0.0.1-SNAPSHOT.jar myapp.jar

# Update the date of the jar file (important if we work with static resources such as images)
RUN sh -c "touch myapp.jar"

CMD ["java", "-jar", "myapp.jar"]

