
## Docker Reference

#### Set up redis on localhost:6379

```bash
    # Create network of type bridge with name redis_network
    docker network create -d bridge redis_network

    # Create docker container on PORT 6379
    docker run --name redis -d --network redis_network -p 6379:6379 redis

    # Create docker image from Dockerfile 
    docker build -f Dockerfile -t {name of image} .
```
