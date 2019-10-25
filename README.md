# CodeChain RPC Go

CodeChain RPC Go is a Go library that calls RPC to a CodeChain node.

## How to install

```bash
go get -u github.com/CodeChain-io/codechain-rpc-go
```

## Example

```Go
package main

import (
	"fmt"
	rpc "github.com/CodeChain-io/codechain-rpc-go"
)
func main() {
	rpc.Init("https://corgi-rpc.codechain.io/")
	fmt.Println(rpc.Version())
}

```

## How to run linter

Make sure you run `revive` before creating a PR to the repo

### Install

```sh
go get -u github.com/mgechev/revive
```

### Run

```sh
revive -config revive.toml
```