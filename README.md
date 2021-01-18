# Windows setup guide

## Win10

Run `.\Win10\_run.bat` as administrator

## Chocolatey

### Install software

Run `.\Chocolatey\_run.bat` as administrator

### Export installed software

Run on PowerShell as administrator

```bash
choco list -lo -r -y | % { $_.Split('|') | select -First 1 } | % { "choco install -y " + $_ } | Out-File .\installed.ps1
```

## Manual installation

- Acronis True Image 2019
- Allway Sync
- Affinity
  - Designer
  - Photo
- Apache
  - Tomcat
- Atom
- Audacity
- Auslogics Disk Defrag
- Battle.net
  - Hearthstone
  - Overwatch
- balenaEtcher
- Cheat Engine
- Docker Desktop
- Epic Games
  - Phoenix Point
- File Shredder
- FileZilla
- Firefox
- Foxit Reader
- GitKraken
- Google Chrome
- HandBrake
- Hearthstone Deck Tracker
- Hyper.js
- Inkscape
- IObit
  - Uninstaller
  - Driver Booster
- JDownloader
- JetBrains
  - Intellij Ultimate
  - PhpStorm
  - PyCharm
- League of Legends
- Logitech Options
- Malwarebytes
- MEGASync
- Microsoft
  - Excel
  - Outlook
  - PowerPoint
  - Word
- Mp3tag
- Notepad++
- Player.me
- Postman
- ProtonVPN
- PuTTY
- qBittorrent
- Razer
  - Cortex
  - Surround
  - Synapse
- Resilio Sync
- Shift
- Snagit 2019
- Signal
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
- TeamSpeak
- TeamViewer
- Vivaldi
- VLC media player
- Win32 Disk Imager
- WinDirStat
- WinPcap
- WinRAR
- Wireshark

## Microsoft Store

- MALClient
- Your Phone
- Ubuntu
