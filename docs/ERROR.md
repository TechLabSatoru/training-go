## package <> is not in GOROOT

- Error Message

    - GOROOTが適切に設定されておらず、`go get`コマンドで外部モジュールを取得したパッケージが異なる場所に格納されている.

```shell
# go test
go: downloading golang.org/x/sync v0.1.0
# github.com/TechLabSatoru/training-go
main_test.go:10:2: package golang/x/sync/errgroup is not in GOROOT (/usr/local/go/src/golang/x/sync/errgroup)
FAIL    github.com/TechLabSatoru/training-go [setup failed]
```

- Solution

```shell
# GOROOTのパスを確認する.
$ go env
```
