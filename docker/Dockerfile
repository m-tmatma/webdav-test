FROM ubuntu:20.04

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install  --fix-missing -y nginx nginx-extras
COPY ./dav.conf /etc/nginx/conf.d/

EXPOSE 80
CMD [ "nginx", "-g", "daemon off;" ]
