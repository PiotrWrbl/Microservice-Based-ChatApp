# Microservice-Based-ChatApp

--DESCRIPTION--

This is a Chat appication that is build in microservice architecture (scheme of it is on the picture below). Communication between services is carried out by RabbitMQ queuing system. 
The application runs in Docker Containers, and is addapted to work on a cluster in docker swarm mode.
Frondend of the application is made using Angular and backend was written in NestJS. Authorization and chat service use Postgres database. 

<img width="685" alt="image" src="https://github.com/PiotrWrbl/Microservice-Based-ChatApp/assets/131017880/c94cc313-304f-4686-bda2-90a678a6eb9c">


--PROJECT_FILE_STRUCTURE--

apps folder contains Backend (NestJs)

chatApp contains Frontend (Angular)

--HOW_TO_RUN--

To run the application using docker you have to type:

docker-compose up

To shut the application use:

docker-compose down

To run app in docker swarm mode you have to use docker-compose-deploy file (It contains elements necessary to run app in swarm network). 

App is available at port 4200:

http://localhost:4200/
