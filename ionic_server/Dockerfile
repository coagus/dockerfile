FROM ubuntu:latest

MAINTAINER Christian Agustin <correo@christianagustin.com>

ENV NODE_VERSION=9.6.1 \
    NPM_VERSION=5.6.0 \
    IONIC_VERSION=3.19.1 \
    CORDOVA_VERSION=8.0.0

RUN apt-get update &&  \
    apt-get install -y git curl && \
    curl --retry 3 -SLO "http://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz" && \
    tar -xzf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 && \
    rm "node-v$NODE_VERSION-linux-x64.tar.gz" && \
    npm install -g npm@"$NPM_VERSION" && \
    npm install -g cordova@"$CORDOVA_VERSION" ionic@"$IONIC_VERSION" && \
    npm cache clear --force && \
    git config --global user.email "networker@christianagustin.com" && \
    git config --global user.name "Christian Agustin" && \
    git clone https://github.com/coagus/ecommerce.git && \
    cd ecommerce

WORKDIR ecommerce
EXPOSE 8100 8100
CMD ["ionic", "serve"]
