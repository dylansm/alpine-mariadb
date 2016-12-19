# alpine-mariadb
Docker image based on alpine-linux mariadb

# build image
```
docker build -t dylansm/alpine-mysql .
docker run -it --rm -v $(pwd):/app -p 3306:3306 dylansm/alpine-mysql
```

# Usage
```
docker run -it --name my-mariadb -p 3306:3306 -v $(pwd):/app -e MYSQL_DATABASE=admin -e MYSQL_USER=tony -e MYSQL_PASSWORD=dpa\*12d -e MYSQL_ROOT_PASSWORD=111111 dylansm/alpine-mariadb
```

It will create a new db, and set mysql root password(default is 111111)
