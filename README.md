# Proto



## How to generate file user.proto
protoc --proto_path=proto/user --go_out=gen/go/user --go_opt=paths=source_relative --go-grpc_out=gen/go/user --go-grpc_opt=paths=source_relative proto/user/user.proto

when error get package, use it
go env -w GOPRIVATE=gitlab.com/bykarya-proto/* && go env -w GONOSUMDB=gitlab.com/bykarya-proto/* && go env -w GONOPROXY=gitlab.com/bykarya-proto/*
##
