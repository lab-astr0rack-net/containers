FROM ubuntu:latest

RUN apt update && DEBIAN_FRONTEND=noninteractive apt install iptables iproute2 curl ca-certificates sudo unzip nodejs git -y

run echo '192.168.55.2   postgres.lab.astr0rack.net' >> /etc/hosts
