# Windows 11 user script

```powershell
Set-WinHomeLocation -GeoID 39 # 244 for US
Get-WinHomeLocation
New-ItemProperty -Path "HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Advanced" -Name "ShowTaskViewButton" -Value 0 -Force 
Get-AppxPackage *WebExperience* | Remove-AppxPackage
Set-ItemProperty -Path "HKCU:\Control Panel\Desktop" -Name WallPaper -Value ''
Set-ItemProperty -Path "HKCU:\Software\Microsoft\Windows\CurrentVersion\Explorer\Wallpapers" -Name BackgroundType -Type DWORD -Value 1
Set-ItemProperty -Path "HKCU:\Control Panel\Colors" -Name Background -Value "0 0 0"
winget install --id Microsoft.Powershell --source winget
winget install --id Brave.Brave
set-ItemProperty -Path 'HKLM:\SOFTWARE\WOW6432Node\Microsoft\Windows\CurrentVersion\Uninstall\Microsoft Edge' -Name 'NoRemove' -value 0
Get-AppxPackage⁣ Microsoft. OneDrive | Remove-AppxPackage
start https://github.com/LeDragoX/Win-Debloat-Tools
winget install --id=Microsoft.VCRedist.2015+.x64  -e
winget install -e --id Oracle.VirtualBox
```
