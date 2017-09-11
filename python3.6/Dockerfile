#################################
# Dockerfile for Alpine Python3 #
#################################
 
FROM python:3.6-alpine
MAINTAINER Desprit <a.bondarev.it@gmail.com>

RUN apk add --update \
  musl-dev \
  build-base \
  bash \
  linux-headers \
  vim \
  && rm /var/cache/apk/*

RUN pip install --upgrade pip
RUN ln -s /usr/include/locale.h /usr/include/xlocale.h
