<!-- omit in toc -->
My Scoop Bucket
==========
[README English Ver.](README.md)

[![MIT licensed][shield-license]][mit]

自分用のバケットです。  
使いたい人がいればどうぞご自由に。


<!-- omit in toc -->
目次
-----------------
<details>
<summary>show</summary>

- [必要条件](#必要条件)
- [インストール](#インストール)
  - [バケットのインストール](#バケットのインストール)
- [使い方](#使い方)
  - [バージョンチェック](#バージョンチェック)
- [バージョニング](#バージョニング)
- [ライセンス & 作者](#ライセンス--作者)
</details>


必要条件
------------
詳細は[Scoopのリポジトリ][scoop]を見てください。
- Windows 7 SP1+ / Windows Server 2008+
- [PowerShell 5][pw5] (or later, include [PowerShell Core][pw_core]) and [.NET Framework 4.5][dot_net_dl] (or later)
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


バージョニング
-----
[SemVer][semver]のガイドラインに則ってバージョン管理しています。  
リリースは以下の形式で行われます。
```
<major>.<minor>.<patch>
```
- 大きな変更や後方互換性のない場合は `<major>` (`<minor>` と `<patch>` もリセット) を上げます。
- 後方互換性があり機能性を追加した場合は `<minor>` (`<patch>` もリセット) を上げます。
- 後方互換性を伴うバグ修正をした場合 `<patch>` を上げます。


ライセンス & 作者
-------
[![MIT licensed][shield-license]](LICENSE)  
Copyright &copy; 2021, ClaudiaHeart



[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
[mit]: https://opensource.org/licenses/MIT
[scoop]: https://github.com/lukesampson/scoop
[pw5]: https://aka.ms/wmf5download
[pw_core]: https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6
[dot_net_dl]: https://www.microsoft.com/net/download
[semver]: http://semver.org/
