FROM ubuntu:latest

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install iptables iproute2 ca-certificates curl sudo ansible virtualenv git -y

RUN curl -L https://github.com/bitwarden/clients/releases/download/cli-v2023.5.0/bw-linux-2023.5.0.zip -o bw.zip && unzip bw.zip && mv bw /usr/bin/ && rm bw.zip
