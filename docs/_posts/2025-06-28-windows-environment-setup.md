---
title:  "Windows環境構築"
date:   2025-06-28 05:18:50 +0900
categories: 環境構築 Windows
tags:   WSL Docker VSCode
---

## 前提
- Windows 11 Pro

## インストール

### WSL2
PowerShellを「管理者として実行」で起動して、以下のコマンドを実行する。

```powershell
wsl --install
```

### Docker Desktop
[ここ](https://www.docker.com/ja-jp/get-started/){:target="_blank"} からインストーラをダウンロードして、インストールする。

### VS Code
[ここ](https://code.visualstudio.com/download){:target="_blank"} からインストーラをダウンロードして。インストールする。

インストール後、VS Codeを起動して、拡張機能``` WSL ```をインストールする。

完了後、Windowsを再起動する。

## 参考サイト
- [WSL2](https://learn.microsoft.com/ja-jp/windows/wsl/install){:target="_blank"}
