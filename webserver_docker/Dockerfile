FROM ubuntu:18.04
LABEL Description="This image is being used for bootcamp exercise"  MAINTAINER="rohit <rohit.mahipal@tothenew.com>" 
RUN apt-get update
RUN apt-get upgrade -y
RUN apt install nginx -y
RUN apt install curl -y
RUN apt install net-tools -y
RUN apt install vim -y
RUN apt install wget -y
RUN rm /etc/nginx/sites-enabled/default
#COPY basic /etc/nginx/sites-enabled/basic
COPY mysite /etc/nginx/sites-enabled/rohit
RUN mkdir -p /var/www/html/rohit
COPY ./rohit/ /var/www/html/rohit
EXPOSE 80
CMD ["nginx", "-g", "daemon on;"]
