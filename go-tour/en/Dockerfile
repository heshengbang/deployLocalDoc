FROM golang:1.9

MAINTAINER heshengbang "yunshixin8521894@sohu.com"

ADD docker-entrypoint.sh /
RUN chmod +x /docker-entrypoint.sh

EXPOSE 3999
WORKDIR $GOPATH

CMD ["/docker-entrypoint.sh"]
