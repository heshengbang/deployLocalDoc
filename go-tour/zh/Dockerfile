FROM golang:1.9

MAINTAINER heshengbang "yunshixin8521894@sohu.com"

RUN go get -u github.com/Go-zh/tour/gotour \
    && chmod +x /docker-entrypoint.sh \
    && chmod +x $GOPATH/bin/gotour

ADD docker-entrypoint.sh /

EXPOSE 3999
WORKDIR $GOPATH

CMD ["/docker-entrypoint.sh"]
