# Windows 11 user script

```powershell
Set-WinHomeLocation -GeoID 39 # 244 for US
Get-WinHomeLocation
New-ItemProperty -Path "HKCU:\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\Advanced" -Name "ShowTaskViewButton" -Value 0 -Force 
Get-AppxPackage *WebExperience* | Remove-AppxPackage

```
