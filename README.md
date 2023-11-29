# go-expert-desafio-clean-architecture

Fazer a listagem das orders com endpoint rest[x], query graphQL [x], endpoint gRPC[x].

## Comandos

### Para ativar ou desativar contêineres docker

##### make init

##### make down

### Para ativar ou parar contêineres docker novamente

##### make start

##### make stop

### Para criar ou apagar migrações

##### make migrate or make migratedown

### Para executar todos os serviços

##### go run main.go wire_gen.go

### Para executar MySQL

##### docker compose exec mysql bash

##### after execute: mysql -p

### Para gerar pasta pb de protocol buffer e grpc

##### protoc --go_out=. --go-grpc_out=. internal/infra/grpc/protofiles/order.proto

### Para acessar o cliente EVANS do gRPC

##### evans -r repl

    - Digite: package pb
    - Digite: service order_service
    - Digite: call CreateOrder or ListOrders



### Para acessar RabbitMQ

##### Acesse localhost:15672

admin: guest
pass: guest
