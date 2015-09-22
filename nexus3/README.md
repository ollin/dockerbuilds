nexus 3.0.0-M5
==============

docker image 

https://support.sonatype.com/entries/96157708-Nexus-3-0-Technology-Preview-Milestone-5-Release-

Usage example:

```
sudo docker run -d -p 8081:8081 --name nexus3 ollin/nexus3
```

- wait for a few seconds and open the browser at http://localhost:8081/
- Don't use it in a production environment! It is a technical preview!

- If you want to use the docker registry feature you need to open the port defined in the Docker Connector Configuration

http://books.sonatype.com/nexus-book/3.0/reference/docker.html#docker-ssl-connector

```
sudo docker run -d -p 8081:8081 -p 18443:18443 --name nexus3 ollin/nexus3
```
