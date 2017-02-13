# Sandbox

## 構築手順（簡易版）

- hostsファイルに書き込み権限をつける
- 以下の必要なものをインストールする
- `vagrant up` コマンドを実行
- `ssh vagrant@ming.dev` でssh接続

## 必要なもの

### Vagrant

公式サイト
http://www.vagrantup.com/

### VirtualBox

公式サイト
https://www.virtualbox.org/

### plugin

CLIで以下を実行

`vagrant plugin install vagrant-hostsupdater`

hostsに開発domainの情報を書き込んでくれる

hostsへの書き込みを行うのでパーミッションは良い感じに設定を行う
