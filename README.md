
## Docker Reference

```bash
    # Create network of type bridge with name redis_network
    docker network create -d bridge redis_network

    # Create docker container on PORT 6379
    docker run --name redis -d --network redis_network -p 6379:6379 redis

    # Create docker image from Dockerfile 
    docker build -f Dockerfile -t {name of image} .
    
    # Create postgres container
    docker run -d -p 5432:5432 --name {container name} -e POSTGRES_PASSWORD=test -e POSTGRES_USER=test -e POSTGRES_DB={database name} postgres"

    # Access mysql server from docker container
    docker exec -it mysql mysql -uroot -p
```
