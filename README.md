# My1stDocker

If you would like to see which containers are running:
docker-compose ps

If you would like to see details like ip-adresses, status, running volumes and stuf you can use the following command:
docker inspect docker_db_1

You should not forget that you should not use 'localhost' for your connection to MariaDB/MySQL. It should be the ip-addres of the database container.
