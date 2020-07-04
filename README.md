# ecoji.io source code

Source code for ecoji.io. All of the web page source is in [index.html](index.html).  The web page calls the ecoji go project using web assembly.  The following builds the web assembly file, however building this is not necessary to edit index.html.

```
GOOS=js GOARCH=wasm go build -o main.wasm main.go
```

For local testing, build and run [ths.go](ths.go) for a simple local web server.

```bash
go build -o ths ths.go
./ths &
# open localhost:8080 in a local web browser
# kill process when done
kill %1
```
