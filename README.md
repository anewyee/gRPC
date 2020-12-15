# gRPC

## install

pip install protobuf
pip install protobuf-compiler

### run

python -m grpc_tools.protoc -I=./protos --python_out=./rpc_package --grpc_python_out=./rpc_package ./protos/user_info.proto./