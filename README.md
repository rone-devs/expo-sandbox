# expo-sandbox

expo さわってなんやかんや

[参考記事](https://qiita.com/hidenoritoki/items/9cd972ba102d12faec0e)

## 構築までの手順

本 repo の root にて

```Shell
docker compose build

docker compose run --rm react_native bash --login
```

コンテナログイン後

```Shell
expo init .

? Choose a template: (Use arrow keys)
  ----- Managed workflow -----
  blank                 a minimal app as clean as an empty canvas
❯ blank (TypeScript)    same as blank but with TypeScript configuration
  tabs                  several example screens and tabs using react-navigation
  ----- Bare workflow -----
  minimal               bare and minimal, just the essentials to get you started
  minimal (TypeScript)  same as minimal but with TypeScript configuration
```

完了後コンテナから抜けて下記コマンド

```Shell
docker compose exec react_native ash
```

```Shell
yarn start
```
