# Spring Boot 2.3 with layered Docker image

Simple example to test out the Spring Boot's support for layered Docker images.

Also stealing some ideas from https://phauer.com/2016/version-numbers-continuous-delivery-maven-docker/#create-adocker-image-and-tag-the-imagewith-theversion-number
for how to set version and docker image name.

Usage:
 
```
./mvnw clean package org.apache.maven.plugins:maven-help-plugin:3.2.0:evaluate -Dexpression=version.number -Doutput=./build.version
docker run -it spring-boot-docker
```