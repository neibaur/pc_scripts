# **🛠️ PowerShell commands to use as an administrator**

- **If the windows search feature is not working:**

```powershell
Get-AppxPackage MicrosoftWindows.Client.CBS | Reset-AppxPackage
```

Then reboot and test out the search bar again