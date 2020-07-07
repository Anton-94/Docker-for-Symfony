FROM node:latest

ARG USER_ID

RUN yarn add \
    @symfony/webpack-encore \
    sass-loader \
    node-sass \
    --dev

WORKDIR /var/www/html
RUN usermod -u $USER_ID node
USER node

CMD ["/node_modules/.bin/encore", "dev"]