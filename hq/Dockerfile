FROM php:7.2-apache

RUN \
  apt-get -y update && \
  apt-get install -y git && \
  apt-get clean

ARG HQ_GITHUB_USER
ARG HQ_GITHUB_PASSWORD

RUN git clone https://${HQ_GITHUB_USER}:${HQ_GITHUB_PASSWORD}@github.com/SparkCC/sparkcc-hq.git /var/www/html
