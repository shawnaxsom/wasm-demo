# wasm-demo

See https://github.com/golang/go/wiki/WebAssembly#getting-started

# Install

```
go get -u github.com/shurcooL/goexec
```

# Build
GOOS=js GOARCH=wasm go build -o main.wasm

# Run
goexec 'http.ListenAndServe(`:8080`, http.FileServer(http.Dir(`.`)))'

