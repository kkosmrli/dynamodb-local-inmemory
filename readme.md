# build image
    
    1. extract deps:
        tar xopf dynamodb_local_latest.tar
    2. build docker image:
        docker build -t docker.edge.tmecosys.com/tmde2-dev/dynamodb-local:latest .

# push image
    docker push docker.edge.tmecosys.com/tmde2-dev/dynamodb-local:latest

# run image
    docker run -d -i -t -p 8000:8000 docker.edge.tmecosys.com/tmde2-dev/dynamodb-local:latest

# dynamodb shell (for debugging and such)
    http://localhost:8000/shell
