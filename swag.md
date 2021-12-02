~$ go get github.com/swaggo/swag/cmd/swag

$ swag init -g .main.go -o ./swagger

$ swag init --parseDependency -d src -g main.go -o ./swagger
