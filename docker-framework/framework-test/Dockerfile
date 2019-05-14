FROM 192.168.1.184:8081/docker-dev-local/docker-framework:latest

MAINTAINER mengke mengke@jfrogchina.com

ADD war/*.war /home/exec/apache-tomcat-8.5.40/webapps/swampup.war

CMD /bin/bash -c cd /home/exec; /home/exec/apache-tomcat-8.5.40/bin/catalina.sh run
