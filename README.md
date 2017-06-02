# My1stDocker

If you would like to see which containers are running:
docker-compose ps

You should see probably:
     Name                    Command              State               Ports
---------------------------------------------------------------------------------------
docker_db_1       docker-entrypoint.sh mysqld     Up      0.0.0.0:3306->3306/tcp
docker_phpfpm_1   docker-php-entrypoint php-fpm   Up      0.0.0.0:9000->9000/tcp
docker_web_1      nginx -g daemon off;            Up      443/tcp, 0.0.0.0:8080->80/tcp

If you would like to see details like ip-adresses, status, running volumes and stuf you can use the following command:
docker inspect docker_db_1

You should not forget that you should not use 'localhost' for your connection to MariaDB/MySQL. It should be the ip-addres of the database container.
