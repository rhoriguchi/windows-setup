# Windows setup guide

## Win10
```
powershell.exe -NoProfile -ExecutionPolicy Bypass -File Win10.ps1 -preset Win10Preset.txt
```

## Chocolatey
Install software
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

.\Chocolatey.ps1
```

Export installed software
```
choco list -lo -r -y | % { $_.Split('|') | select -First 1 } | % { "choco install " + $_ + " -y" } | Out-File .\Chocolatey.ps1
```

## Manual installation
  - Affinity
    - Designer
    - Photo
  - Evolve
  - League of Legends
  - MALClient
  - Microsoft Office
  - Veeam Agent for Microsoft Windows
