FROM ubuntu:latest

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install unzip iptables iproute2 ca-certificates curl sudo ansible virtualenv git -y && pip3 install ansible-pylibssh
