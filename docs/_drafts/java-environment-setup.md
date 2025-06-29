---
title:  "Java開発環境構築"
categories: 環境構築 開発
tags: Java
---

### OpenJDK 21
以下のコマンドでインストールする。
```bash
sudo apt install openjdk-21-jdk
```
.bashrcを開く。
```bash
vi ~/.bashrc
```
.bashrcの末尾に以下を追加する。
```bash
JAVA_HOME=$(readlink -f /usr/bin/javac | sed "s:/bin/javac::")
export JAVA_HOME
PATH=$PATH:$JAVA_HOME/bin
export PATH
```
シェルを再起動する。
```bash
exec $SHELL -l
```
