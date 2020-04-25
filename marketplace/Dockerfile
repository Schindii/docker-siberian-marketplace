FROM debian:10

MAINTAINER dev@xtraball.com

RUN apt-get update
RUN apt-get install -y curl wget zip unzip vim git
RUN apt-get install -y php7.3-cli php7.3-curl php7.3-mbstring php7.3-gd php7.3-fpm

WORKDIR /var/www/html

COPY ./wrapper.sh /usr/bin/wrapper.sh
RUN chmod +x /usr/bin/wrapper.sh

CMD /usr/bin/wrapper.sh