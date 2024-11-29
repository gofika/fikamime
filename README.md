# fikamime

A simple and lightweight MIME type detection library for Go, with support for over 800 file extensions.

## Features

- Fast MIME type lookup by file extension
- Support for common file formats
- Zero dependencies
- Thread-safe

## Installation

```shell
go get github.com/gofika/fikamime
```

## Usage

```go
package main

import (
    "fmt"
    "github.com/gofima/fikamime"
)

func main() {
    // Get MIME type by file extension
    mimeType := fikamime.TypeByExtension(".pdf")
    fmt.Println(mimeType) // Output: application/pdf
    // Common examples
    fmt.Println(fikamime.TypeByExtension(".jpg")) // image/pjpeg
    fmt.Println(fikamime.TypeByExtension(".png")) // image/png
    fmt.Println(fikamime.TypeByExtension(".mp4")) // video/mp4
    fmt.Println(fikamime.TypeByExtension(".docx")) // application/vnd.openxmlformats-officedocument.wordprocessingml.document
}
```