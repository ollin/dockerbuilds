# VERSION 2

FROM ollin/ubuntu-14.04-oracle-jdk8
MAINTAINER Oliver Nautsch <oliver.nautsch@gmail.com>

RUN apt-get update
RUN apt-get install -y -q curl unzip
RUN curl -s get.gvmtool.net | bash

ADD run /opt/run
ONBUILD RUN ["/opt/run", "selfupdate"]

ENTRYPOINT ["/opt/run"]