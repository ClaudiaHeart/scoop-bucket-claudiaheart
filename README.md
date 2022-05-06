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
  - [check version](#check-version)
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
### check version
```sh
.\scoop\bin\checkver.ps1 * -dir bucket
```
### update version
```sh
.\scoop\bin\checkver.ps1 * -dir bucket -u
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
[scoop]: https://github.com/lukesampson/scoop
[pw5]: https://aka.ms/wmf5download
[pw_core]: https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6
[dot_net_dl]: https://www.microsoft.com/net/download
[semver]: http://semver.org/
