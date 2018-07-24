FROM php:7.0-apache

RUN apt update -y \
  && echo "deb http://packages.dotdeb.org jessie all" >> /etc/apt/sources.list \
  && echo "deb-src http://packages.dotdeb.org jessie all" >> /etc/apt/sources.list \
  && apt install -y wget \
  && wget https://www.dotdeb.org/dotdeb.gpg \
  && apt install -y gnupg \
  && apt-key add dotdeb.gpg \
  && apt update -y

RUN a2enmod rewrite
