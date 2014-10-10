vertx
=====

docker image 

-  http://vertx.io/

Usage example:

- myApp.zip is your vertx module
- the module contains a vertx module with an httpServer listening at port 8080
- your Dockerfile: 

```
FROM ollin/vertx
MAINTAINER dev devi <dev.devi@devsmailserver.com>

VOLUME /home/developer
ADD myApp.zip /home/developer/myApp.zip
EXPOSE 8080

WORKDIR /home/developer
CMD ["vertx", "runzip", "myApp.zip"]
```
