### Go

```
protoc --go_out=paths=source_relative:./gen \
  --go-grpc_out=paths=source_relative:./gen \
  --proto_path=. \
  --go_opt=Muser.proto=gen/userpb \
  --go_opt=Mauth.proto=gen/authpb \
  --go-grpc_opt=Muser.proto=gen/userpb \
  --go-grpc_opt=Mauth.proto=gen/authpb \
  auth.proto user.proto
```