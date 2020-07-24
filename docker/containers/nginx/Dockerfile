FROM nginx:latest

WORKDIR /var/www/html
RUN chown -R nginx:nginx /var/www/html

COPY ./default.conf /etc/nginx/conf.d/default.conf

CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80