# micro-go

[![ci](https://github.com/Akagi201/micro-go/actions/workflows/ci.yml/badge.svg)](https://github.com/Akagi201/micro-go/actions/workflows/ci.yml)

micro service framework in Go

## Features

* Monorepo - Sharing code between microservies
* [PGV](https://github.com/envoyproxy/protoc-gen-validate) - input validation
* [cli](https://cli.urfave.org/) - urfave/cli
* [koanf](https://github.com/knadh/koanf) - env, config
* [logr](https://github.com/go-logr/logr) - log interface
* [zap](https://github.com/uber-go/zap) - log implementation
* [grpc](google.golang.org/grpc) - use pure GRPC
* [req](https://github.com/imroc/req) - http client
* [errors](https://github.com/cockroachdb/errors) - error handling
* [ent](https://entgo.io/) - Graph-Based ORM
* [wire](https://github.com/google/wire) - dependency injection
* [govvv](https://github.com/ahmetb/govvv)
* [golangci](https://golangci-lint.run/) - lint tools
* [buf](https://buf.build) - protobuf management
* [super-linter](https://github.com/github/super-linter) - lint everything
* [tableflip](https://github.com/cloudflare/tableflip) - graceful process restart
* graphql: [rejoiner](https://github.com/google/rejoiner) [gqlgen](https://gqlgen.com/)

## third-party tools

```sh
# k8s tool similar to helm  (optional)
# generate fill k8s yaml files from overlays
brew install kustomize
# kubeval - validate one or more Kubernetes config files(optional)
brew tap instrumenta/instrumenta
brew install kubeval
# Manage Your lk8s In Style!
brew install derailed/k9s/k9s
# buf: proto tool https://buf.build/docs/tour-1
brew tap bufbuild/buf
brew install buf
```

golang tools

```sh
# go better build tool
go install github.com/ahmetb/govvv@latest
# for static check/linter
go install github.com/golangci/golangci-lint/cmd/golangci-lint@latest

# fetch protoc plugins into $GOPATH
go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest

# to add tags to go struct
go install github.com/srikrsna/protoc-gen-gotag@latest

# goup checks if there are any updates for imports in your module.
# the main purpose is using it as a linter in continuous integration or in development process.
# Usage: goup -v -m ./...
go install github.com/rvflash/goup@latest
```
