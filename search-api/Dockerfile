FROM golang:1.12.7

RUN adduser --disabled-password --gecos '' api
USER api

WORKDIR /go/src/elastic-docker
COPY . .

RUN go install -v ./...

CMD [ "elastic-docker" ]