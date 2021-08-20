FROM tomcat:jdk8
RUN apt update
RUN apt install maven -y
COPY webappwar /usr/local/tomcat/webapps/
WORKDIR /usr/local/tomcat/webapps
RUN mvn package
RUN mv target/mywebapp.war .
