# Get Started with dfuse graphQL API over gRPC 

### Before you begin
- Visit [golang gRPC prerequisites](https://grpc.io/docs/quickstart/go.html#prerequisites)
- Then make sure that `protoc` is accessible from your $PATH

### Get the source code
- `git clone https://github.com/dfuse-io/example-graphql-grpc.git`
- `git clone https://github.com/dfuse-io/graphql-over-grpc.git`

### Generates the graphql.pb.go
- `protoc -I graphql-over-grpc graphql/graphql.proto --go_out=plugins=grpc:./example-graphql-grpc`

### Getting project dependencies
- `cd example-graphql-grpc`
- `go mod init main`
- `go mod tidy` 

### Run it!
- Visit [https://app.dfuse.io](https://app.dfuse.io) to get YOUR_API_KEY 
- `go run main.go YOUR_API_KEY_HERE`
