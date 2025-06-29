---
title:  "Ubuntu環境構築"
date:   2025-06-29 17:57:23 +0900
categories: 環境構築 Linux
tags:   Ubuntu Jekyll Git
---

## 前提
- [Windows環境構築]({% post_url 2025-06-28-windows-environment-setup %})
- Ubuntu上で、以下のコマンドを実行する。
    ```bash
    sudo apt-get update
    ```

## インストール

### Jekyll
Rubyと必要なパッケージをインストールする。
```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```
.bashrcに設定を追加するため、以下のコマンドを実行する。
```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
JekyllとBundlerをインストールする。
```bash
gem install jekyll bundler
```

### Git
コマンドがインストールされているか確認する。
```bash
git --version
```
インストールされていない場合、以下のコマンドでインストールする。
```bash
sudo apt-get git
```
以下のコマンドで、```user.email```と```user.name```を設定する。
```bash
git config --global user.email <メールアドレス>
git config --global user.name <ユーザ名>
```

## 参考サイト
- [Jekyll](https://jekyllrb.com/docs/installation/ubuntu/){:target="_blank"}
