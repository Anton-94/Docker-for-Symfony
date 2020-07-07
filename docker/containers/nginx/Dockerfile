FROM nginx:latest

COPY ./default.conf /etc/nginx/conf.d/default.conf

WORKDIR /var/www/html

CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80