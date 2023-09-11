
```bash
docker run --rm -it --name grpc-ruby -v $(dirname PWD):/app bash
```

```bash
cd app/ruby
bundle install
grpc_tools_ruby_protoc -I ../proto --ruby_out=lib --grpc_out=lib ../proto/greet.proto
```

```bash
docker exec -it grpc-ruby bash
```

```bash
cd app/ruby

```