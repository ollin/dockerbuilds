nexus 3.0.0-7M
==============

docker image 

https://support.sonatype.com/hc/en-us/articles/215781148-Nexus-Repository-Manager-3-0-Milestone-7-Release-

Usage example:

```
docker run -d -p 8081:8081 --name nexus3 ollin/nexus3
```

- wait for a few seconds and open the browser at http://localhost:8081/
- Don't use it in a production environment! It is a technical preview!

- If you want to use the docker registry feature you need to open the port defined in the Docker Connector Configuration

http://books.sonatype.com/nexus-book/3.0/reference/docker.html#docker-ssl-connector

```
docker run -d -p 8081:8081 -p 18443:18443 --name nexus3 ollin/nexus3
```
