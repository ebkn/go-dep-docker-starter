FROM golang:1.11.1-alpine3.8

COPY src /go/src/api

WORKDIR /go/src/api

RUN apk update \
  && apk add --no-cache git \
  && go get -u github.com/golang/dep/... \
  && dep ensure
