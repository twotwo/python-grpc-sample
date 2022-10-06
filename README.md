# gRPC Sample Code for Learning

## setup for running

    # newer for poetry
    curl -sSL https://install.python-poetry.org | POETRY_VERSION=1.2.1 python3 -
    # install dependency
    poetry install
    poetry shell
    pre-commit install
    pre-commit run -a

### Generate protobuf files

    $ cd grpc-errors
    $ python -m grpc_tools.protoc --proto_path=./ --python_out=./stub --grpc_python_out=./stub ./hello.proto

### Run client and server

    $ python server.py &
    $ python client.py

## gRPC Error

fork from [grpc-errors](https://github.com/avinassh/grpc-errors/tree/master/python)