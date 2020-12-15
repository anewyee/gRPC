# Python gRPC 示例

## link 
https://grpc.io/docs/quickstart/python.html

## install

pip install protobuf
pip install protobuf-compiler

## compile 
使用以下命令编译:
python -m grpc_tools.protoc -I./ --python_out=. --grpc_python_out=. ./helloworld.proto
复制代码生成了两个文件：

helloworld_pb2.py 此文件包含生成的 request(HelloRequest) 和 response(HelloReply) 类。
helloworld_pb2_grpc.py 此文件包含生成的 客户端(GreeterStub)和服务端(GreeterServicer)的类。

## run

首先运行服务端

python greeter_server.py

然后运行客户端

python greeter_client.py

>  output
Greeter client received: Hello, goodspeed!
