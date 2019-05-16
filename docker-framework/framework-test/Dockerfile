FROM docker-release.art.local/docker-framework:latest

MAINTAINER mengke mengke@jfrogchina.com

ADD war/*.war /home/exec/apache-tomcat-8.5.40/webapps/xxl-job-executor-sample-spring-2.0.2-20190515.145751-1.war

CMD /bin/bash -c cd /home/exec; /home/exec/apache-tomcat-8.5.40/bin/catalina.sh run
