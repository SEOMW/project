FROM httpd:latest

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y apache2 git
RUN git clone https://github.com/SEOMW/mycloud.git
RUN cp -r mycloud/* /var/www/html/
CMD ["apachectl", "-D", "FOREGROUND"]
