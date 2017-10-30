FROM ensemblorg/ensembl-vep

USER root

# Install Node
RUN apt-get update && apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash

RUN apt-get -y install nodejs

COPY consumer.js /tmp/consumer.js

WORKDIR /tmp

RUN npm install amqplib

#USER vep
