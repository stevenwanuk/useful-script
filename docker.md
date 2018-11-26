# run mssql-server-linux-developer
docker run -d -p 1433:1433 -e sa_password=root -e ACCEPT_EULA=Y microsoft/mssql-server-linux-developer

# run redis
docker run -p 6379:6379 -d redis

# run configserver
docker-compose up -d configserver

# export container to file
docker export 688b8867a45b >> a.tar