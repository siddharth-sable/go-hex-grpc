# go-hex-grpc
 This GoLang project is built using the Hexagonal Port and Adapters architectural pattern and incorporates gRPC communication and Docker containerization. The Hexagonal architecture, also known as Ports and Adapters architecture, provides a modular and flexible approach for designing and organizing applications.
 ## Project structure
 
 ```
 .
├── Dockerfile
├── README.md
├── cmd
│   └── main.go
├── docker-compose.yaml
├── go.mod
├── go.sum
├── grpc_entrypoint.sh
├── internal
│   ├── adapters
│   │   ├── app
│   │   │   └── api
│   │   │       └── api.go
│   │   ├── core
│   │   │   └── arithmetic
│   │   │       ├── arithmetic.go
│   │   │       └── arithmetic_test.go
│   │   └── framework
│   │       ├── left
│   │       │   └── grpc
│   │       │       ├── pb
│   │       │       │   ├── arithmetic_svc_grpc.pb.go
│   │       │       │   └── number_msg.pb.go
│   │       │       ├── proto
│   │       │       │   ├── arithmetic_svc.proto
│   │       │       │   └── number_msg.proto
│   │       │       ├── rpc.go
│   │       │       ├── rpc_test.go
│   │       │       └── server.go
│   │       └── right
│   │           └── db
│   │               └── db.go
│   └── ports
│       ├── app.go
│       ├── core.go
│       ├── framework_left.go
│       └── framework_right.go
└── testdb
    └── init.sql

16 directories, 23 files
 ```
