## Task 1 - Dockerize the Application

Python-React Apps.

1. created docker container for backend, nginx proxy server and Front end React app.
/smartcow/api

Backend service is running on port 50000

Docker build -t pythonapp .
docker run -p 5000:5000 -d pythonapp

/smartcow/sys-stats
Front end React app is running on 3000

Docker build -t pythonapp .
docker run -p 3000:3000 -d nodeapp

2. configuration for the proxy information added into default.conf file under nginx folder

3.docker-compose up --build

This will spin up the containers and also expose the ports so you can test on your browser. After the containers are up, you can type docker ps -a in the command line to see the running containers,
and the ports they are running on:

docker ps 



