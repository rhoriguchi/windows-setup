# Windows setup guide

## Win10
Run `.\Win10\_run.bat` as administrator

## Chocolatey
### Install software
Run on Powershell
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```
Run `.\Chocolatey\InstalledSoftware.ps1` as administrator

### Export installed software
```
choco list -lo -r -y | % { $_.Split('|') | select -First 1 } | % { "choco install " + $_ + " -y" } | Out-File .\Chocolatey\InstalledSoftware.ps1
```

## Manual installation
  - Affinity
    - Designer
    - Photo
  - Battle.net
  - Evolve
  - League of Legends
  - MALClient
  - Microsoft Office
  - Veeam Agent for Microsoft Windows
