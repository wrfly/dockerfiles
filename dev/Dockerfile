FROM ubuntu
MAINTAINER wrfly <mr.wrfly@gmail.com>

RUN apt-get update && apt-get upgrade -y \
    && apt-get install -y iptables vim xxd iftop \
    tcpdump dnsutils iputils-* nmap netcat atop \
    silversearcher-ag mtr iotop ngrep iptraf bc \
    strace traceroute iproute2 lsof curl wget \
    python unzip zip psmisc htop tzdata locate \
    && echo "Asia/Singapore" > /etc/timezone \
    && apt-get clean \
    && apt-get autoclean \
    && apt-get autoremove

CMD ["bash"]
