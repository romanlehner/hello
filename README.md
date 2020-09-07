# Working with Modules

## Creating a module

A module allows you to manage resources independently from GOPATH. Dependencies are referenced by the [go.mod](go.mod) file and dependecy operations such as `go get` or `go build` will download them accordingly. 

The module of this project was initialized as follows:

```bash
go mod init github.com/romanlehner/hello
```

## Naming conventions

... in progress

## Loading a module as dependency

The following command will add the newest version of the `greeting` module:

```bash
go get github.com/romanlehner/greetings
```

A version can be specified as follows:

```bash
go get github.com/romanlehner/greetings@v1.0.0
```

## Updating major version

... in progress

https://blog.golang.org/v2-go-modules

## Clena up module

```bash
go mod tidy
```
This command make sure that unused modules are removoed from both [go.sum](go.sum) and [go.mod](go.mod) files. 