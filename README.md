GOOS=linux GOARCH=amd64 go build -o goserver main.go

docker build . -t goserver:latest

docker run -p 8080:8080 goserver
