<!-- omit in toc -->
My Scoop Bucket
==========
[README 日本語版](README_JP.md)

[![MIT licensed][shield-license]][mit]

This Scoop Bucket for me to use.  
But if anyone wants to use this Scoop Bucket, you can use it.


<!-- omit in toc -->
Table of Contents
-----------------
<details>
<summary>show</summary>

- [Requirements](#requirements)
- [Install](#install)
  - [install bucket](#install-bucket)
- [Usage](#usage)
  - [Check Version](#check-version)
  - [Update Version](#update-version)
  - [Check URL](#check-url)
  - [Describe](#describe)
  - [Missing Check Version](#missing-check-version)
  - [Format JSON](#format-json)
- [Versioning](#versioning)
- [License & Author](#license--author)
</details>


Requirements
------------
See [Scoop Repository][scoop] for details.
- Windows 7 SP1+ / Windows Server 2008+
- [PowerShell 5][pw5] (or later, include [PowerShell Core][pw_core]) and [.NET Framework 4.5][dot_net_dl] (or later)
- PowerShell must be enabled for your user account e.g. `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`


Install
-----
### install bucket
```sh
scoop bucket add ClaudiaHeart https://github.com/ClaudiaHeart/scoop-bucket-claudiaheart
```


Usage
-----
- [Scoop/bin][scoop_bin]
- [App Manifest Autoupdate][scoop_autoupdate]
### Check Version
```ps
.\scoop\bin\checkver.ps1 -a <App> -d <Dir> -v <Version>
.\scoop\bin\checkver.ps1 -a * -d bucket
```
### Update Version
```ps
.\scoop\bin\checkver.ps1 -a <App> -d <Dir> -v <Version> -Update
.\scoop\bin\checkver.ps1 -a * -d bucket -Update
```
### Check URL
```ps
.\scoop\bin\checkurls.ps1 -a <App> -d <Dir>
.\scoop\bin\checkurls.ps1 -a * -d bucket
```
### Describe
```ps
.\scoop\bin\describe.ps1 -a <App> -d <Dir>
.\scoop\bin\describe.ps1 -a * -d bucket
```
### Missing Check Version
```ps
.\scoop\bin\missing-checkver.ps1 -a <App> -d <Dir> -v <Version>
.\scoop\bin\missing-checkver.ps1 -a * -d bucket
```
### Format JSON
```ps
.\scoop\bin\formatjson.ps1 -a <App> -d <Dir>
.\scoop\bin\formatjson.ps1 -a * -d bucket
```


Versioning
-----
[SemVer][semver] is used here as a guideline for version control.  
Releases are made in the following format
```
<major>.<minor>.<patch>
```
- Breaking changes bump `<major>` (and reset `<minor>` & `<patch>`)
- Backward compatible changes bump `<minor>` (and reset `<patch>`)
- Bug fixes bump `<patch>`


License & Author
-------
[![MIT licensed][shield-license]](LICENSE)  
Copyright &copy; 2021, ClaudiaHeart



[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
[mit]: https://opensource.org/licenses/MIT
[scoop]: https://github.com/ScoopInstaller/Scoop
[scoop_bin]: https://github.com/ScoopInstaller/Scoop/tree/master/bin
[scoop_autoupdate]: https://github.com/ScoopInstaller/Scoop/wiki/App-Manifest-Autoupdate
[pw5]: https://aka.ms/wmf5download
[pw_core]: https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6
[dot_net_dl]: https://www.microsoft.com/net/download
[semver]: http://semver.org/
