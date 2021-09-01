FROM centos:latest

LABEL Author = Edris
LABEL Role = Devops Engineer

RUN yum -y update && yum clean all
RUN yum install httpd -y
RUN systemctl enable httpd.service

ADD ./app1.html /var/www/html/

EXPOSE 90

#CMD systemctl -D FOREGROUND

ENV servername app1-server
ENV container docker
