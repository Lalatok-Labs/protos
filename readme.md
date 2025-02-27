## Use Go

```
$ git submodule add https://github.com/Lalatok-Labs/protos.git proto

$ protoc \          
    -Iproto/common \
    --go_out=internal/proto \
    --go-grpc_out=internal/proto \
    proto/common/ping.proto

```