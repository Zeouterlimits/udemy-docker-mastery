docker volume create pgdata
docker run --name gavin-postgres-1 -e POSTGRES_PASSWORD=mysecretpassword -d -v pgdata:/var/lib/postgresql/data postgres:9.6.1
docker run --name gavin-postgres-2 -e POSTGRES_PASSWORD=mysecretpassword -d -v pgdata:/var/lib/postgresql/data postgres:9.6.2