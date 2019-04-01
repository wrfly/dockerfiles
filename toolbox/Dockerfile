FROM ubuntu
LABEL maintainer="wrfly <mr.wrfly@gmail.com>"
RUN export DEBIAN_FRONTEND=noninteractive \
    && apt-get update && apt-get upgrade -y \
    && apt-get install -y iptables vim xxd iftop \
    tcpdump dnsutils iputils-* nmap netcat atop \
    silversearcher-ag mtr iotop ngrep iptraf bc \
    strace traceroute iproute2 lsof curl wget \
    python unzip zip psmisc htop tzdata locate \
    tmux sudo git \
    && git clone https://github.com/gpakosz/.tmux.git \
    && ln -s -f .tmux/.tmux.conf \
    && cp .tmux/.tmux.conf.local . \
    && echo "Asia/Singapore" > /etc/timezone \
    && apt-get clean \
    && apt-get autoclean \
    && apt-get autoremove

CMD ["sleep", "infinity"]
