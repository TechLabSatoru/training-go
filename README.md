## Goのプロジェクト開発

```shell
# プロジェクトの初期化
$ go mod init github.com/TechLabSatoru/training-go

# Goの実行（ビルドせず）
$ go run .
```

## 開発環境の構築

```shell
# dockerコンテナを作成します.
$ docker compose up -d

# dockerコンテナの中に入ります.
$ docker compose exec -it golang bash

# dockerコンテナを削除します.
$ docker compose down --rmi all --volumes --remove-orphans
```
