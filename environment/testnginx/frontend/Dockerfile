#Docker file ubuntu imaage for testapp frontend 
FROM ubuntu:18.04
MAINTAINER deepak1825@gmail.com
RUN apt-get -y update
ADD config /opt
ENV TZ="Asia/Kolkata"
RUN apt-get -y install tzdata
RUN apt-get -y install `cat /opt/packages`
RUN apt-get -y install `cat /opt/mypackages`
ADD code /var/www/html
#COPY code /var/www/html--copy the folder 
EXPOSE 80
ENV BACKENDLB=test
CMD ["nginx", "-g", "daemon off;"]
#ENTRYPOINT