# dockerfile
En este repositorio se encuentra como instalar docker en un ubuntu y Dockerfile para proyectos

## Instalar Docker en Ubuntu
> sudo su

> apt-get install -y apt-transport-https ca-certificates curl software-properties-common

> curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add -

> add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

> apt-get update

> apt-get install -y docker-ce
