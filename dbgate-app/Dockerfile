FROM nginx:stable-alpine

RUN apk add --no-cache apache2-utils
RUN mkdir -p /etc/nginx/auth
RUN htpasswd -cb /etc/nginx/auth/.htpasswd admin 123456
COPY ./config/nginx.conf /etc/nginx/conf.d/default.conf
