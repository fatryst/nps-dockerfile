FROM alpine:3.9
MAINTAINER fatryst <fatryst@gmail.com>

WORKDIR /
ENV NPS_VERSION v0.26.10
ENV NPS_RELEASE_URL https://github.com/ehang-io/nps/releases/download/$NPS_VERSION/linux_amd64_server.tar.gz

RUN set -x && \
        wget --no-check-certificate ${NPS_RELEASE_URL} && \ 
        tar xzf linux_amd64_server.tar.gz && \
    rm linux_amd64_server.tar.gz

VOLUME /conf

ENTRYPOINT ["/nps"]  
