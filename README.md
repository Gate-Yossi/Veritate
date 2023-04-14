Veritate
====

読み方:ティタウィン

## Description
フロントエンド関係のフレームワーク等の動作検証用リポジトリになります。


## React

### 開発する場合

```bash
pushd react
docker compose build
docker compose up -d
```

ブラウザで `localhost:3000` にアクセスする。

### ビルドしたコンテンツをnginxで確認する場合

```bash
docker compose build
docker compose up -d
docker compose run --rm front sh -c "cd /src/app && yarn build"
```

ブラウザで `localhost:8080` にアクセスする。
