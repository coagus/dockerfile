FROM alpine:3.9

ENV NODE_VERSION=10.14.2-r0

WORKDIR /project

RUN apk add nodejs=$NODE_VERSION npm=$NODE_VERSION && \
    rm -rf /var/cache/apk/* 

EXPOSE 3000

#CMD ["node"]