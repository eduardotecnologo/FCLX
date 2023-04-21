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
