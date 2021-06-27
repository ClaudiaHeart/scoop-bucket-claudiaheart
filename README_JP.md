My Scoop Bucket
==========
[README English Ver.](README.md)

自分用のバケットです。
使いたい人がいればどうぞご自由に。

[![MIT licensed][shield-license]](#)


目次
-----------------

  * [必要条件](#必要条件)
  * [インストール](#インストール)
  * [使い方](#使い方)
  * [ライセンス](#ライセンス)


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


ライセンス
-------
This Repository is licensed under the [MIT](LICENSE) license.
Copyright &copy; 2021, ClaudiaHeart



[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
