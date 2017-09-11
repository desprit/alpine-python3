###################################
# Dockerfile for Alpine Python3.5 #
###################################
 
FROM alpine:latest
MAINTAINER Desprit <a.bondarev.it@gmail.com>

RUN apk add --update \
  musl-dev \
  build-base \
  python3 \
  python3-dev \
  bash \
  linux-headers \
  vim \
  && rm /var/cache/apk/*

RUN cd /usr/bin \
  && ln -sf easy_install-3.5 easy_install \
  && ln -sf idle3.5 idle \
  && ln -sf pydoc3.5 pydoc \
  && ln -sf python3.5 python \
  && ln -sf python-config3.5 python-config \
  && ln -sf pip3.5 pip

RUN pip install --upgrade pip
RUN ln -s /usr/include/locale.h /usr/include/xlocale.h
