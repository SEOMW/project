FROM nginx:latest

ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && \
    apt-get install -y nginx git
RUN git clone https://github.com/SEOMW/mycloud.git
RUN cp -r mycloud/* /usr/share/nginx/html
CMD ["nginx", "-g", "daemon off;"]
