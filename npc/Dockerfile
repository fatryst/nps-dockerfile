FROM alpine:3.9
MAINTAINER fatryst <fatryst@gmail.com>

WORKDIR /
ENV NPC_VERSION v0.26.8
ENV NPC_RELEASE_URL https://github.com/ehang-io/nps/releases/download/$NPC_VERSION/linux_amd64_client.tar.gz

RUN set -x && \
        wget --no-check-certificate ${NPC_RELEASE_URL} && \ 
        tar xzf linux_amd64_client.tar.gz && \
    rm linux_amd64_client.tar.gz

VOLUME /conf

ENTRYPOINT ["/npc"]
