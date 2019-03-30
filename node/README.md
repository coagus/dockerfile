# Node Server

Create a node server contanainer for develop or deploy your project.

## Spects

Alpine Linux
> # cat /etc/os-release 
NAME="Alpine Linux"
ID=alpine
VERSION_ID=3.9.2
PRETTY_NAME="Alpine Linux v3.9"
HOME_URL="https://alpinelinux.org/"
BUG_REPORT_URL="https://bugs.alpinelinux.org/"

Node
> node --version
v10.14.2

NPM
> # npm --version
6.4.1

## Build, Run & Enter

..* Build image
> docker build --tag=project:node .

..* Run container
> docker run -it -d -p 3000:3000 --name=node project:node

..* Enter the container
> docker exec -it node /bin/sh

## Size of container

docker image ls
REPOSITORY          TAG                 IMAGE ID            CREATED              SIZE
project             node                d1db8dd700fd        About a minute ago   46.8MB
alpine              3.9                 5cb3aa00f899        3 weeks ago          5.53MB