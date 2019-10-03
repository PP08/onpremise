FROM nginx
WORKDIR /etc/nginx
RUN apt update
RUN apt install python-certbot-nginx -y
RUN apt install cron -y
RUN apt install vim -y
EXPOSE 80
EXPOSE 443