FROM ubuntu:22.04

WORKDIR /var/www/html

RUN apt-get update && \
           apt-get install -y nginx

RUN rm -f /var/www/html/index.nginx.html

COPY app/* /var/www/html/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
