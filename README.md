# protoc-gen-hprose


## Install

Use `go get` to install the code generator:

```bash
go get github.com/cuigh/protoc-gen-hprose
```

You will also need:

* [protoc](https://github.com/google/protobuf), the protobuf compiler. You need version 3+.
* [protoc-gen-go](https://github.com/golang/protobuf/), the Go protobuf generator plugin. Get this with `go get github.com/golang/protobuf/protoc-gen-go`.

## Usage

Just like **grpc**:

```bash
protoc --go_out=. --hprose_out=. hello.proto
```

Service interfaces and client proxies were generated into a separate file `[name].hprose.go`:

```
hello.hprose.go
hello.pb.go
hello.proto
```