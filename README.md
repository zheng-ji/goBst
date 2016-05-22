## goBst

[![Build Status](https://travis-ci.org/zheng-ji/goBst.svg)](https://travis-ci.org/zheng-ji/goBst)
[![GoDoc](https://godoc.org/github.com/zheng-ji/goBst?status.svg)](https://godoc.org/github.com/zheng-ji/goBst)

A threadsafe Binary Search Tree written in Go

线程安全的二叉查找树


Installation
-------------

```
go get github.com/zheng-ji/goBst
```

Example
-------

```go
import (
	"fmt"
	bst "github.com/zheng-ji/goBst"
)

func main() {
	s := bst.NewBstTs()
	s.Insert(8)
	s.Insert(4)
	s.Insert(5)

	if s.Exists(4) {
        fmt.Println("exists")
    }

	s.ShowInOrder()
	s.ShowPreOrder()
	s.ShowPostOrder()
}
```

License
-------

MIT

