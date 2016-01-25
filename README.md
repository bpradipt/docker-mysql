Dockerize mysql. The example Dockerfile is tested on PowerPC LE system
#Build
docker build -t mysql .
#Run
docker run -itd -e MYSQL_ROOT_PASSWORD=password -e MYSQL_USER=user -e MYSQL_PASSWORD=pass -e MYSQL_DB=test -P mysql 
