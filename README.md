# Windows setup guide

## Win10
Run `.\Win10\_run.bat` as administrator

## Chocolatey

### Install software
Run on PowerShell as administrator
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

choco feature enable -n allowGlobalConfirmation
```
Run `.\Chocolatey.bat` as administrator

### Export installed software
Run on PowerShell as administrator
```
choco list -lo -r -y | % { $_.Split('|') | select -First 1 } | % { "choco install " + $_ } | Out-File .\Chocolatey.bat
```

## Manual installation
- Affinity
- Battle.net
- Designer
- IObit Uninstaller
- JDownloader
- League of Legends
- MALClient
- Microsoft Office
- Photo
- Player.me
- Razer Synapse
- Spotify
- Synergy
- Visual Studio Code
