## Ejecutamos el Dockerfile
> docker build -t coagus/ecommerce .

## Levantamos el contenedor
> docker run -it -d -p 8100:8100 --name=ecommerce coagus/ecommerce

## Entramos al contenedor
> docker exec -it ecommerce /bin/bash

## Dentro del Contenedor Ejecutamos
> ionic serve
