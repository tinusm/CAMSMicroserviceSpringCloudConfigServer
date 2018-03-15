FROM java
MAINTAINER tanmay ambre
COPY ./target/configserver-0.0.1-SNAPSHOT.jar /usr/local/configserver/
RUN ls -al /usr/local/configserver
EXPOSE 11013
VOLUME /logs
WORKDIR /usr/local/configserver
ENTRYPOINT java -Xmx512m -jar configserver-0.0.1-SNAPSHOT.jar > /logs/config_server_system.out.log
