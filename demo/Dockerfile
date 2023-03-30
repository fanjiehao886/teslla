FROM java:openjdk-8u111-jdk
COPY ./target/demo-0.0.1-SNAPSHOT.jar /usr/src/app.jar
VOLUME /tmp
EXPOSE 8080
CMD ["java", "-jar", "app.jar"]
LABEL maintainer="Jack Fan"
RUN bash -c 'touch /usr/src/app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/usr/src/app.jar"]