# FCLX

Integração  ChatGPT com Zap!

## Docker e Containers e Microsserviço do ChatGPT
Ctrl+shift+p
$go:install

## Go migrations
$migrate create -ext=mysql -dir=sql/migrations -seq init
$sqlc generate 

## off containner runnig
$docker rm -f $(docker ps -a -q)

## Runing chatservice
$docker-compose exec chatservice bash

## Generate li tiktoken.a
$cargo build --release

##
/go/src# go run cmd/chatservice/main.go

## Install protoc Ubuntu
$sudo apt-get install autoconf automake libtool curl make g++ unzip

$apt-get install -y protobuf-compiler
$protoc --version

## Setup gRPC in WSL
## No arquivo makefile incluir a flag  --experimental como abaixo:

- protoc --go_out=. --go-grpc_out=. proto/chat.proto --experimental_allow_proto3_optional

## Realizar a instalação do protoc-gen-go

Linux (WSL2) ou dentro do container:
apt install protoc-gen-go 

No Mac deve ser instalado os dois pacotes abaixo:

brew install protoc-gen-go
brew install protoc-gen-go-grpc 

Rodar dentro do container:

go get google.golang.org/grpc/cmd/protoc-gen-go-grpc
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc