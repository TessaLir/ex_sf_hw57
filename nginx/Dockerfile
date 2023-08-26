FROM ubuntu:latest  

RUN apt-get update  
RUN apt-get install -y nginx  

COPY ./hosts/application.local.conf /etc/nginx/sites-enabled/application.local.conf
COPY ./hosts/example.local.conf /etc/nginx/sites-enabled/example.local.conf
COPY ./hosts/tesska.local.conf /etc/nginx/sites-enabled/tesska.local.conf

WORKDIR /data  
VOLUME /data  

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]