# Go
This is a Go in Docker boilerplate I use myself whenever I start a Go project from scratch.

Enjoy it. Make suggestions if you like so.

# necessary steps
## check doors
- docker-compose.yaml ->
  - check if doors mapping is linking to a free port
  (8000:8000)

## 1st execution:
- comment lines 18 to 20
- execute -> docker exec -it app_any bash
- from the container execute:
  - go mod init your-project-name
  ("your-project-name" is any name you like)
  - go get github.com/satori/go.uuid
  - go get github.com/spf13/cobra-cli

## next executions:
- uncomment lines 18 to 20
- execute once -> docker-compose up --build
(to rebuilt the container with uncommented lines)
- start programing in Go

# have fun using Go -> https://go.dev/solutions/#case-studies