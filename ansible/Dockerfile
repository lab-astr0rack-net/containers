FROM ubuntu:latest

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install unzip iptables iproute2 ca-certificates curl sudo ansible virtualenv git libssh-dev -y && pip3 install ansible-pylibssh

COPY requirements.yml /

RUN ansible-galaxy install -r /requirements.yml --roles-path /etc/ansible/roles && rm /requirements.yml
