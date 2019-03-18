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

## Programmes

- .NET Core
- Acronis True Image 2019
- Allway Sync
- Affinity
  - Designer
  - Photo
- Apache
  - Maven
  - Tomcat
- Atom
- Audacity
- Auslogics Disk Defrag
- Battle.net
  - Hearthstone
  - Overwatch
- balenaEtcher
- Cheat Engine
- Discord
- Docker Desktop
- Driver Booster
- File Shredder
- FileZilla
- Firefox
- Foxit Reader
- GeForce Experience
- Git
- GitKraken
- Google Chrome
- HandBrake
- Hearthstone Deck Tracker
- Hyper.js
- Inkscape
- IObit Uninstaller
- Java JDK 11
- JDownloader
- JetBrains
  - Intellij Ultimate
  - PhpStorm
  - PyCharm
- League of Legends
- Logitech Options
- Malwarebytes
- MEGASync
- Microsoft Office
- Mp3tag
- NordVPN
- Notepad++
- Player.me
- Postman
- PuTTY
- Python 3
- qBittorrent
- Razer
  - Cortex
  - Surround
  - Synapse
- Resilio Sync
- Skype
- Spotify
- StarUML
- Steam
  - Chaos Reborn
  - Doki Doki Literature Club!
  - Dungeon of the Endless
  - FTL: Faster Than Light
  - Middle-earth: Shadow of Mordor
  - Shadowverse
  - Slay the Spire
  - Swords & Soldiers
  - The Binding of Isaac: Rebirth
- Synergy
- TeamViewer
- Telegram
- Vivaldi
- VLC media player
- WhatsApp
- Win32 Disk Imager
- WinDirStat
- WinPcap
- WinRAR
- Wireshark

## Microsoft Store
- MALClient
- Your Phone
