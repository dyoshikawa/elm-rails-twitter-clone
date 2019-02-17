FROM ruby:alpine
MAINTAINER dyoshikawa

RUN apk update
RUN apk add --update --no-cache \
      bash \
      postgresql-client \
      nodejs \
      tzdata
RUN apk add --update --no-cache --virtual=build-dependencies \
      build-base \
      curl-dev \
      linux-headers \
      libxml2-dev \
      libxslt-dev \
      postgresql-dev \
      ruby-dev \
      yaml-dev \
      zlib-dev
RUN gem install bundler
RUN gem install rails

