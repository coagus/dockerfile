FROM alpine

MAINTAINER Christian Agustin <correo@christianagustin.com>

RUN apk update && apk upgrade && \
    apk add --update nodejs && \
    apk add --update git && \
    git clone https://github.com/coagus/srv-web-api-user.git && \
    cd srv-web-api-user && \
    sh init.sh

WORKDIR srv-web-api-user

EXPOSE 3000 3000

CMD ["node", "src/app.js"]
