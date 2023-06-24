FROM jenkins/inbound-agent:3107.v665000b_51092-5

USER root

RUN apt-get update && apt-get install -y \
    apt-transport-https \
    ca-certificates \
    python3 \
    python3-pip \
    curl \
    wget \
    zip \
    unzip

RUN pip3 install awscli --upgrade

RUN curl -fsSL https://get.docker.com | sh
RUN rm -rf /var/lib/apt/lists/*

USER jenkins
