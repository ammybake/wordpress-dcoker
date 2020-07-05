# wordpress-doker
Deploying wordpress with nginx , mysql and let's encrypt in digitalocean.com
we are going to creat two file only !! 
1. Docker-compose.yml 
2. nginx-conf/nginx.conf
everything will be in ~/wordpress directory

# so let's get started

$ mkdir wordpress && cd wordpress

$ mkdir nginx-conf

$ nano nginx-conf/nginx.conf

$ nano .env

MYSQL_ROOT_PASSWORD=your_root_password
MYSQL_USER=your_wordpress_database_user
MYSQL_PASSWORD=your_wordpress_database_password

$ git init

$ nano .gitignore

add .env into it


$ nano .dockerignore


.env
.git
docker-compose.yml
.dockerignore


$ curl -sSLo nginx-conf/options-ssl-nginx.conf https://raw.githubusercontent.com/certbot/certbot/master/certbot-nginx/certbot_nginx/_internal/tls_configs/options-ssl-nginx.conf

When everythins is setsup just type
 
 
$ docker-compose up -d 

Go to the browser https://yoururl.com

--------------------------






