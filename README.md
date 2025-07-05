# interfacer

Interfacer is a Go command line that transforms public methods for a struct into an interface

## Installation

```bash
go install github.com/SeaRoll/interfacer@latest
```

#### Or with tools

```go
//go:build tools
// +build tools

package tools

import (
	_ "github.com/SeaRoll/interfacer/cmd"
)
```

## Usage

```bash
interfacer [flags]

# Usage:
-file string
  The name of the output file. (default "interface.go")
-name string
  The name of the interface to generate. (default "Service")
-path string
  The source package directory to scan. (default ".")
-struct string
  The name of the source struct. (default "service")
```
