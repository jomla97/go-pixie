go-pixie is a simple Go wrapper for the [Pixie SMS API](https://www.pixie.se/Home/Index).

# Getting started

## Installation
```
go mod init github.com/my/repo
go get github.com/jomla97/go-pixie
```

## Importing
``` go
import "github.com/jomla97/go-pixie"
```

## Complete example
``` go
px := pixie.NewClient("username", "password")

err := px.Send("sender", "+46xxxxxxxxx", "Hello world!\n\nRegards,\ngo-pixie")
if err != nil {
    //Handle error
}
```