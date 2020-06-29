FROM ubuntu:16.04

RUN apt-get update -y && apt-get upgrade -y
RUN apt-get install curl wget -y

RUN curl -fsSL https://code-server.dev/install.sh | sh

EXPOSE 8080

CMD code-server --auth none --port 8080 --bind-addr=0.0.0.0:8080
