<!-- omit in toc -->
My Scoop Bucket
==========
[README English Ver.](README.md)

[![MIT licensed][shield-license]](https://licenses.opensource.jp/MIT/MIT.html)

自分用のバケットです。  
使いたい人がいればどうぞご自由に。


<!-- omit in toc -->
目次
-----------------
- [必要条件](#必要条件)
- [インストール](#インストール)
  - [バケットのインストール](#バケットのインストール)
- [使い方](#使い方)
  - [バージョンチェック](#バージョンチェック)
- [ライセンス & 作者](#ライセンス--作者)


必要条件
------------
詳細は[Scoopのリポジトリ](https://github.com/lukesampson/scoop)を見てください。
- Windows 7 SP1+ / Windows Server 2008+
- [PowerShell 5](https://aka.ms/wmf5download) (or later, include [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6)) and [.NET Framework 4.5](https://www.microsoft.com/net/download) (or later)
- PowerShell must be enabled for your user account e.g. `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`


インストール
-----
### バケットのインストール
```sh
scoop bucket add ClaudiaHeart https://github.com/ClaudiaHeart/scoop-bucket-claudiaheart
```


使い方
-----
### バージョンチェック
```sh
.\scoop\bin\checkver.ps1 * -dir . -u
```


ライセンス & 作者
-------
[![MIT licensed][shield-license]](LICENSE)  
Copyright &copy; 2021, ClaudiaHeart



[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
