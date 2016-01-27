Dockerize mysql. 
#Build
docker build -t mysql .

For building it on PowerPC LE platform do this
docker build -t ppc64le/mysql -f Dockerfile.ppc64le .

#Run
docker run -itd -e MYSQL_ROOT_PASSWORD=password -e MYSQL_USER=user -e MYSQL_PASSWORD=pass -e MYSQL_DB=test -P mysql 
