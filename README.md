#Docker-Spark-Zepplein

1. To start 1 Master and 1 Worker

   docker-compose up -d 

2. To start 1 Master and n workers

   docker-compose up -d && docker-compose scale worker=n

3. Logs
   docker-compose logs

4. Master UI
   a. Find the ip address, docker-machine ip
   b. Got to http://masterip:8080


5. To login into a container

  a. Find container id using, docker ps
  b. Login into the container, 
     docker exec -it conainer-id /bin/bash

6. Zeppelin UI
   http://masterip:8082

7. Shutdown containers
   docker-compose down
