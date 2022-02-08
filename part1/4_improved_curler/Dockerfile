FROM ubuntu:20.04

RUN apt update && apt install -y curl

COPY script.sh .

RUN chmod +x script.sh

ENTRYPOINT  ["./script.sh" ]
