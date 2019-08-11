FROM openjdk:8-jre-alpine

ENV LANG C.UTF-8
RUN mkdir -p /usr/local/bin/gatling && \
    rm -rf /usr/local/bin/gatling/user-files/*
COPY ./app/ /usr/local/bin/gatling/
