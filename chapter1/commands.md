## Build image
docker build . -t node-service

## run docker
docker run -d -p 8080:8080 node-service
### -d for deamon
### -p for forwared container 8080 port to the host 8080. host:container

## login to docker hub
docker login

## Add tag to the image
docker tag ee2122d45b4e mosheeve/node-service:latest

## push the image to the repositorty 
docker push mosheeve/node-service

## Remove the image
docker image rm mosheeve/node-service

## pull the image 
docker pull mosheeve/node-service
