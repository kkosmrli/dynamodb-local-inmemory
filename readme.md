# build image
    
    1. extract deps:
        tar xopf dynamodb_local_latest.tar
    2. build docker image:
        docker build -t docker.edge.tmecosys.com/tmde2-dev/dynamodb-local:latest .

# dynamodb shell (for debugging and such)
    http://localhost:8000/shell
