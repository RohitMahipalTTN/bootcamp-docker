# bootcamp-docker

step 1: 
docker build -t webserver .

step 2:
docker run -itd -t webserver_container -p 8081:80 webserver

step 3:
docker ps -a

step 4:
docker images

step 4: (OPTIONAL)
docker exec -it webserver_container /bin/bash


