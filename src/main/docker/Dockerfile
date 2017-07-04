FROM store/oracle/serverjre:8

EXPOSE 8080

#install Spring Boot artifact
VOLUME /tmp
ADD springboot_docker-1.0.war springboot_docker-1.0.war 
RUN sh -c 'touch /springboot_docker-1.0.war'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/springboot_docker-1.0.war"]