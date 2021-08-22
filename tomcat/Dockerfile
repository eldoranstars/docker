FROM tomcat:jdk8
RUN apt update
RUN apt install maven -y
RUN mv /usr/local/tomcat/webapps.dist/* /usr/local/tomcat/webapps
COPY webappwar /usr/local/tomcat/webapps/
WORKDIR /usr/local/tomcat/webapps
RUN mvn package
RUN mv target/mywebapp.war /usr/local/tomcat/webapps/
EXPOSE 8080
