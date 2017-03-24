FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD configSeverDemo-0.0.1-SNAPSHOT.jar configServer.jar
RUN sh -c 'touch /configServer.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /configServer.jar" ]
