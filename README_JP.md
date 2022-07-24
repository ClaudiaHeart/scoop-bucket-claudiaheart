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
  - [バージョン更新](#バージョン更新)
  - [URLをチェックする](#urlをチェックする)
  - [ハッシュ値をチェックする](#ハッシュ値をチェックする)
  - [概要を出力する](#概要を出力する)
  - [バージョンチェックと自動更新が設定されているかチェックする](#バージョンチェックと自動更新が設定されているかチェックする)
  - [アプリマニフェストのJSONをフォーマットする](#アプリマニフェストのjsonをフォーマットする)
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
```pwsh
scoop bucket add ClaudiaHeart https://github.com/ClaudiaHeart/scoop-bucket-claudiaheart
```


使い方
-----
- [Scoop/bin][scoop_bin]
- [App Manifest Autoupdate][scoop_autoupdate]
### バージョンチェック
```pwsh
.\scoop\bin\checkver.ps1 -a <App> -d <Dir> -v <Version>
.\scoop\bin\checkver.ps1 -a * -d bucket
```
### バージョン更新
```pwsh
.\scoop\bin\checkver.ps1 -a <App> -d <Dir> -v <Version> -u
.\scoop\bin\checkver.ps1 -a * -d bucket -u
```
### URLをチェックする
```pwsh
.\scoop\bin\checkurls.ps1 -a <App> -d <Dir>
.\scoop\bin\checkurls.ps1 -a * -d bucket
```
### ハッシュ値をチェックする
```pwsh
.\scoop\bin\checkhashes.ps1 -a <App> -d <Dir>
.\scoop\bin\checkhashes.ps1 -a * -d bucket
```
### 概要を出力する
```pwsh
.\scoop\bin\describe.ps1 -a <App> -d <Dir>
.\scoop\bin\describe.ps1 -a * -d bucket
```
### バージョンチェックと自動更新が設定されているかチェックする
```pwsh
.\scoop\bin\missing-checkver.ps1 -a <App> -d <Dir> -v <Version>
.\scoop\bin\missing-checkver.ps1 -a * -d bucket
```
### アプリマニフェストのJSONをフォーマットする
```pwsh
.\scoop\bin\formatjson.ps1 -a <App> -d <Dir>
.\scoop\bin\formatjson.ps1 -a * -d bucket
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
Copyright &copy; 2022, ClaudiaHeart



[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
[mit]: https://licenses.opensource.jp/MIT/MIT.html
[scoop]: https://github.com/ScoopInstaller/Scoop
[scoop_bin]: https://github.com/ScoopInstaller/Scoop/tree/master/bin
[scoop_autoupdate]: https://github.com/ScoopInstaller/Scoop/wiki/App-Manifest-Autoupdate
[pw5]: https://aka.ms/wmf5download
[pw_core]: https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6
[dot_net_dl]: https://www.microsoft.com/net/download
[semver]: https://semver.org/lang/ja/
