# VERSION 2

FROM ollin/gvm
MAINTAINER Oliver Nautsch <oliver.nautsch@gmail.com>

RUN ["/opt/run", "install", "vertx", "2.1.2"]
RUN ["/opt/run", "default", "vertx", "2.1.2"]

ADD run /opt/run

CMD ["version"]
ENTRYPOINT ["/opt/run"]