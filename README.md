# 🌳 Go Bonzai™ Default `help` Command

[![GoDoc](https://godoc.org/github.com/rwxrob/help?status.svg)](https://godoc.org/github.com/rwxrob/help)
[![License](https://img.shields.io/badge/license-Apache2-brightgreen.svg)](LICENSE)

This is the default help originally included with the [Go Bonzai
package](https://github.com/rwxrob/bonzai) itself but factored out so
that it's `Version` tag could be consistent with other Bonzai branches
(which correspond to git tags by convention). This also allows other
(potentially better) `help.Cmd` to be developed without a substantial
bias one way or another.

## Install

```go
package z

import (
	Z "github.com/rwxrob/bonzai/z"
	"github.com/rwxrob/help"
)

var Cmd = &Z.Cmd{
	Name:     `z`,
	Commands: []*Z.Cmd{help.Cmd}, // usually first
}
```

## Other Examples

* <https://github.com/rwxrob/z> - the one that started it all
