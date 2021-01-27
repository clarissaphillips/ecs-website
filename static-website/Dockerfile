FROM ubuntu:latest
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install apache2 -y
RUN apt-get install nano -y
EXPOSE 80
RUN rm -rf /var/www/html
RUN mkdir /var/www/html
COPY . /var/www/html
CMD apachectl -D FOREGROUND