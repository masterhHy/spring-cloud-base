FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD api-gateway-1.0-SNAPSHOT.jar app.jar
ADD wait-for-it.sh /wait-for-it.sh
#RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
EXPOSE 18000