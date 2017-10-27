# DockerSwarmAndRabbitMQ
A test of Docker Swarm and RabbitMQ

## Setup RabbitMQ
1. Download and install RabbitMQ
1. Run RabbitMQ Docker Container
1. Install amqp.node with npm
npm install amqplib

## Create a swarm of consumers (workers)
1. Setup a docker machine
1. SSH into docker machine
1. Run docker swarm init

## Run producer script to send messages to workers
