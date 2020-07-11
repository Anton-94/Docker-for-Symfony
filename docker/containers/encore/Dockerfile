FROM node:14

WORKDIR /var/www/html

ARG USER_ID

RUN yarn add \
    @symfony/webpack-encore \
    sass-loader \
    node-sass \
    --dev

RUN usermod -u $USER_ID node
USER node

CMD ["/node_modules/.bin/encore", "dev"]