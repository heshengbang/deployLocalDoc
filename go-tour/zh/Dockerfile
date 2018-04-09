FROM golang:1.9

MAINTAINER heshengbang "yunshixin8521894@sohu.com"

RUN go get -u github.com/Go-zh/tour/gotour

ADD docker-entrypoint.sh /
RUN chmod +x /docker-entrypoint.sh
RUN chmod +x $GOPATH/bin/gotour

EXPOSE 3999
WORKDIR $GOPATH

CMD ["/docker-entrypoint.sh"]
