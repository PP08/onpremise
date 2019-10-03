FROM nginx
WORKDIR /etc/nginx
COPY . /etc/nginx/conf.d/
RUN apt update
RUN apt install python-certbot-nginx -y
RUN apt install cron -y
RUN apt install vim -y
RUN crontab ./conf.d/renewssl
EXPOSE 80
EXPOSE 443