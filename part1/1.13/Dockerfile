FROM golang:alpine

ENV REQUEST_ORIGIN=http://localhost:5000

EXPOSE 8080

RUN apk add --no-cache git && \
	git clone https://github.com/docker-hy/material-applications.git /apps

WORKDIR /apps/example-backend

RUN go build

CMD ["./server"]
