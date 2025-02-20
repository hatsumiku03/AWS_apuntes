FROM alpine:3.14

RUN apk add --no-cache nginx php php7-fpm

RUN echo "<p>Holi :3</p><br><?php phpinfo(); ?>" > /var/www/localhost/htdocs/index.php

RUN mkdir -p /run/nginx && \
    mkdir -p /etc/nginx/conf.d/ && \
    echo 'server { listen 80; server_name localhost; root /var/www/localhost/htdocs; index index.php index.html; location / { try_files $uri $uri/ /index.php; } }' > /etc/nginx/conf.d/default.conf

EXPOSE 80

CMD php-fpm7 && nginx -g 'daemon off;'