FROM java:8-jre-alpine
VOLUME /tmp

ADD *.jar app.jar
# RUN bash -c 'touch /app.jar'
RUN ln -sf /usr/share/zoneinfo/Asia/Jakarta  /etc/localtime
EXPOSE 10001

#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/.urandom","-jar","/app.jar"]

ENTRYPOINT java ${JAVA_OPTS} -Djava.security.egd=file:/dev/./urandom -jar /app.jar