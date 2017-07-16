# packer-itamae

# description

PackerとItamaeによる環境構築の自動化&コード管理
各環境でItamae実行に必要な各種設定を行い、Itamaeを実行する
対応環境

* AWS
* Docker

# how to use

環境変数で各種設定を管理しているので設定が必要です。(direnv推奨)

* ITAMAE_REPO # Itamae管理ディレクトリの指定

* AWS_ACCESS_KEY_ID # AWS利用の場合
* AWS_SECRET_ACCESS_KEY　# AWS利用の場合

コマンド
onlyのオプションで実行対象の環境を指定します。

```
packer build -only=docker manifest.json
```
