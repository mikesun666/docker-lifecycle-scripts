FROM ubuntu:latest

MAINTAINER mengke mengke@jfrogchina.com

RUN /bin/bash -c cd ~; cd /home ; mkdir -p exec
ADD java/jdk-8u212-linux-x64.tar.gz /home/exec
#RUN /bin/bash -c cd /home/exec; mv /home/exec/jdk1* /home/exec/jdk8
ENV JAVA_HOME=/home/exec/jdk1.8.0_212
RUN sed "/securerandom.source=/{s/file:\/dev\/random/file:\/dev\/urandom/}" /home/exec/jdk1.8.0_212/jre/lib/security/java.security -i

ADD tomcat/apache-tomcat-8.5.40.tar.gz /home/exec
#RUN /bin/bash -c cd /home/exec; mv /home/exec/apache-tomcat-8.* /home/exec/tomcat
ADD tomcat/server.xml /home/exec/apache-tomcat-8.5.40/conf
ENV CATALINA_HOME=/home/exec/apache-tomcat-8.5.40

CMD /bin/bash -c cd /home/exec; /home/exec/apache-tomcat-8.5.40/bin/catalina.sh run
