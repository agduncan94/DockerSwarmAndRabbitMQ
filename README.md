# DockerSwarmAndRabbitMQ
A test of Docker Swarm and RabbitMQ

## Setup RabbitMQ
1. Download and install RabbitMQ
1. Run RabbitMQ Docker Container

## Create a shared volume
docker volume create --name HeliVolume

## Consumer
### Build consumer Docker image
cd consumer
docker build -t "consumer" .
### Run Consumer
docker run --rm -i -t consumer /bin/bash
./consumer

## Producer
### Build producer Docker image
cd producer
docker build -t "producer" .
### Run Producer
docker run --rm -i -t producer /bin/bash
./producer
