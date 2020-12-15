# gRPC

## install

pip3 install protobuf
pip3 install protobuf-compiler

### run

python3 -m grpc_tools.protoc -I=./protos --python_out=./rpc_package --grpc_python_out=./rpc_package ./protos/user_info.proto./