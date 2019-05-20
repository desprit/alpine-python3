FROM python:3.6-alpine3.9
LABEL maintainer="Desprit <a.bondarev.it@gmail.com>"

RUN apk add --update \
  musl-dev \
  build-base \
  linux-headers \
  && rm /var/cache/apk/*

RUN pip install --upgrade pip
RUN ln -s /usr/include/locale.h /usr/include/xlocale.h

RUN pip install pandas