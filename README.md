# Goes - 复制自字节跳动的gopkg仓库的gopool，独立仓库

## Introduction

`gopool` is a high-performance goroutine pool which aims to reuse goroutines and limit the number of goroutines.

It is an alternative to the `go` keyword.

## Features

- High Performance
- Auto-recovering Panics
- Limit Goroutine Numbers
- Reuse Goroutine Stack

## QuickStart

```shell
go get -u github.com/bytepowered/goes
```

Just replace your `go func(){...}` with `goes.Go(func(){...})`.

old:
```go
go func() {
	// do your job
}()
```

new:
```go
goes.Go(func(){
	/// do your job
})
```