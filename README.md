# gRPC Client-Server Communication in Go

## Introduction
This project demonstrates a Client-Server communication model using gRPC in Go. It showcases different communication patterns such as unary, server streaming, client streaming, and bidirectional streaming. gRPC, which uses Protocol Buffers for serialization, provides a robust and efficient way to communicate between distributed services, especially in microservices architectures.

## Purpose of the Project
The project was created to showcase how gRPC can simplify and enhance communication between services. It focuses on improving performance, reducing latency, and enabling scalability. By using Protocol Buffers instead of JSON, the project also achieves faster data transfer with a smaller payload size, making it ideal for real-time and resource-constrained applications.

## Key Use Cases
- **Microservices Communication**: Allows different microservices to interact efficiently.
- **Real-Time Data Streaming**: Ideal for applications like chat, live notifications, and data streaming.
- **Blockchain and Distributed Systems**: Supports peer-to-peer interactions where asynchronous, bidirectional communication is crucial.

### Features
- **Unary RPC**: A single request and response interaction.
- **Server Streaming RPC**: Server streams multiple responses for a single request.
- **Client Streaming RPC**: Client sends a stream of requests to the server and receives a single response.
- **Bidirectional Streaming RPC**: Both client and server can exchange streams of messages simultaneously.

## Scalability Enhancements
To make this project scalable:
- **Load Balancing**: Deploy multiple server instances with a load balancer.
- **Horizontal Scaling**: Replicate the server to handle more requests.
- **Connection Pooling**: Efficiently manage multiple connections for better resource usage.
- **Data Caching**: Use caching to reduce database load.
- **Fault Tolerance**: Implement retry mechanisms and backup servers for resilience.

---

## Getting Started

### Prerequisites
- **Go**: Version 1.16 or later.
- **gRPC and Protocol Buffers compiler (protoc)**.

### Installation

#### Clone the Repository
```bash
git clone https://github.com/ayussh203/grpc-client-server-golang.git
cd grpc-client-server-golang
```

### Generate Protocol Buffers Code

#### Run the following command to generate Go code from the .proto file:
```bash
protoc --go_out=. --go-grpc_out=. proto/greet.proto
```

### Run the Server

#### To start the server, run:
``` bash
cd server
go run .
```


### Run the Client

#### Open another terminal and run the client:
``` bash
cd client
go run .

```


![image](https://github.com/user-attachments/assets/1f17727f-91fe-44ed-9a42-4dc95d623fb3)
![image](https://github.com/user-attachments/assets/3016da8b-ac4b-4489-b9c0-9f1b3377d110)


