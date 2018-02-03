<p align="center">
  <img src="https://github.com/TakuSemba/grpc-android/blob/master/arts/grpc.png" width="300">
</p>

---

# grpc-go

This is The Proto for this project. send a coffee and receive a coffee.

```proto
syntax = "proto3";

option java_package = "com.takusemba.grpc.android.protos";
option go_package = "protos";

package Coffee;

message CoffeeRequest {
    string name = 1;
}

message CoffeeResponse {
    int32 price = 1;
    string name = 2;
    string message = 3;
}

service Coffee {
    rpc Order (CoffeeRequest) returns (CoffeeResponse) {}
}
```

### how to start

```
go run sever.go
```


### Proto File

see [grpc-proto](https://github.com/TakuSemba/grpc-proto) for the proto file.

### Server Side

see [grpc-go](https://github.com/TakuSemba/grpc-go) for the server side.
