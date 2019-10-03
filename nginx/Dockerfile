FROM nginx
WORKDIR /etc/nginx
COPY ./renewssl /etc/nginx/
RUN apt install python-certbot-nginx -y
RUN apt install cron -y
RUN apt install vim -y
RUN crontab /etc/nginx/renewssl
EXPOSE 80
EXPOSE 443