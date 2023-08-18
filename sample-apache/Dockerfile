FROM httpd:latest

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y apache2
RUN git clone https://github.com/SEOMW/mycloud.git
COPY ./sample-apache/ /var/www/html/
CMD ["apachectl", "-D", "FOREGROUND"]

# 컨테이너 내부의 80 포트와 연결
EXPOSE 80
