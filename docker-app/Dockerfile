FROM docker-release-local2.demo.jfrogchina.com/docker-framework:latest

MAINTAINER mengke mengke8292963@163.com

ADD war/*.war /home/exec/apache-tomcat-8.5.39/webapps/swampup.war

CMD /bin/bash -c cd /home/exec; /home/exec/apache-tomcat-8.5.39/bin/catalina.sh run

