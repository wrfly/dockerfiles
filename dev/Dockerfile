FROM ubuntu
MAINTAINER wrfly <mr.wrfly@gmail.com>

RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y iptables vim xxd \
    tcpdump dnsutils iputils-* nmap netcat \
    strace traceroute iproute2 lsof curl wget \
    python unzip zip psmisc htop tzdata locate \
    && echo "Asia/Singapore" > /etc/timezone \
    && apt-get clean \
    && apt-get autoclean \
    && apt-get autoremove

CMD ["bash"]
