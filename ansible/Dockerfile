FROM ubuntu:latest

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install unzip iptables iproute2 ca-certificates curl sudo ansible virtualenv git libssh-dev python3-paramiko ansible-lint -y

COPY requirements.yml /
RUN ansible-galaxy collection install -p /usr/share/ansible/collections -r /requirements.yml  && rm /requirements.yml
