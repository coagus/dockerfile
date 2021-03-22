# LAMP with Docker
Simple LAMP server for develop quickly.

## Step by step
Download your repository
```sh
mkdir web 
git clone https://github.com/<user>/<php repo>.git web
```
Create your image
```sh
docker build -t <user>/lamp .
```
Run your containter
```sh
docker run -it -d -p 80:80 -p 443:443 -p 3306:3306 --name=dev -v "$(pwd)"/web:/var/www/html <user>/lamp
```
Excecute your script
```sh
docker exec -i dev mysql -u root < ./web/<script folder>/createdb.sql
```
