# Xmondrian-updated
**by Anton Dziavitsyn 2018**  
**[based on original xmondrian by @rolandbouman](https://github.com/rpbouman/xmondrian)**

(current version use mondrian-8.0.0.2-R, and olap4j-1.2.0)

## Introduction
This repository is a build of original [x-mondrian by @rolandbouman](https://github.com/rpbouman/xmondrian), based on latest libs versions (mondrian, olap4j, and others).  
I did not changed anything in original x-mondrian pages.  

## How to use
Just clone this repository, and build it with maven:  
```bash
mvn clean package
```
Also you may run it with Tomcat server in docker container:
```bash
docker run -it --rm -p 8888:8080 -v $PWD/target/web:/usr/local/tomcat/webapps:rw tomcat:8-jre8
```
Then locate xmondrian homepage here:  
(http://localhost:8888/xmondrian)
