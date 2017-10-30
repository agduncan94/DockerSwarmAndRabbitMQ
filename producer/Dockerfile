FROM ubuntu:14.04

USER root

# Install Node
RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash

RUN apt-get -y install nodejs

COPY producer.js /tmp/producer.js

WORKDIR /tmp

RUN npm install amqplib
