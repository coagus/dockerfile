FROM alpine
WORKDIR /src
RUN apk update && apk add git npm && \
    git config --global user.name "Christian Agustin" && \
    git config --global user.email "christian@agustin.gt" && \
    git config --global init.defaultBranch main 
    
# docker build -t coagus/gitmoji .
# docker run -dit --name=gitmoji coagus/gitmoji
# docker run -dit --name=gitmoji -v C:/developer/dockerfile:/src coagus/gitmoji
# docker exec -it gitmoji ash
# npm i -g gitmoji-cli