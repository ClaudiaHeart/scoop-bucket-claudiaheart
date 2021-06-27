My Scoop Bucket
==========
[README 日本語版](README_JP.md)

This Scoop Bucket for me to use.
But if anyone wants to use this Scoop Bucket, you can use it.

[![MIT licensed][shield-license]](#)


Table of Contents
-----------------

  * [Requirements](#requirements)
  * [Install](#Install)
  * [Usage](#usage)
  * [License](#license)


Requirements
------------
See [Scoop Repository](https://github.com/lukesampson/scoop) for details.
- Windows 7 SP1+ / Windows Server 2008+
- [PowerShell 5](https://aka.ms/wmf5download) (or later, include [PowerShell Core](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-6)) and [.NET Framework 4.5](https://www.microsoft.com/net/download) (or later)
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
.\scoop\bin\checkver.ps1 * -dir . -u
```


License
-------
This Repository is licensed under the [MIT](LICENSE) license.
Copyright &copy; 2021, ClaudiaHeart



[shield-license]: https://img.shields.io/badge/license-MIT-blue.svg
