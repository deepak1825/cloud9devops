#Docker file apache imaage for testapp frontend 
FROM centos:7
MAINTAINER deepak1825@gmail.com
#RUN useradd deepak
#USER deepak
#WORKDIR /app
RUN yum -y update 
RUN yum -y install httpd
ADD code /var/www/html
#COPY code /var/www/html--copy the folder 
EXPOSE 80
ENV BACKENDLB=test
CMD ["apachectl", "-D", "FOREGROUND"]
#ENTRYPOINT
