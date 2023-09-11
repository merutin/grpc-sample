
```bash
protoc --go_out=./pb --go_opt=paths=source_relative --go-grpc_out=./pb --go-grpc_opt=paths=source_relative --proto_path=../proto greet.proto
```

```bash
go run greeter_server/main.go
```

```bash
go run greeter_client/main.go
```