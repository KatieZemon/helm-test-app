## Generated Java Jar
mvn package (Jar in target folder)
small one is code you wrote (b/c default thing that maven does). spring says that's not very useful so it also produces large one which contains all dependencies

## Push Image in Docker
Docker file > building on top of base image: Googled Java 11 Base Image https://hub.docker.com/_/openjdk

docker build -t helm-test-app:1.0.0 .  // Needed openjdk7 installed. Just built the image. Container is running instance of image

## Run the image in Docker
// i is interactive, rm means if program dies remove the container, demo-app is container name, demo-app is img name
// Feature of docker is security. tcp port is not accessible outside docker container. p is for publish or redirect. could be 8081:8081
docker run -it --rm --name helm-test-app-cntr -p 8082:8081 helm-test-app:1.0.0

## Access the Image
http://localhost:8082/hi


## Deploy with Kubectl


## Deploy with Helm



