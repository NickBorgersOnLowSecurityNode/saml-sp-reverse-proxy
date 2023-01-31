FROM debian:bullseye-slim

RUN apt update && apt-get upgrade -y && apt install --no-install-recommends -y apache2 libapache2-mod-auth-mellon && apt-get clean

RUN a2enmod proxy && a2enmod proxy_http

CMD apachectl -D FOREGROUND
