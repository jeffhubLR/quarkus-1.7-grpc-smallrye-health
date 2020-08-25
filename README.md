# Quarkus 1.7 with gRPC and smallrye health issue

This project was generated from code.quarkus.io, selecting quarkus-grpc and smallrye health extensions.

After following the [gRPC Getting Started](https://quarkus.io/guides/grpc-getting-started) guide, the service was started using `mvn compile quarkus:dev`

Calls to the gRPC service succeed:

`grpcurl -plaintext -proto=src/main/proto/helloworld.proto localhost:9000 helloworld.Greeter.SayHello`

But the gRPC healthcheck fails:

`curl http://localhost:8080/health`
