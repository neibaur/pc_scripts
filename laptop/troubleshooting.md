# 🛠️ PowerShell commands (run as Administrator)

## Fix Windows Search 🔎

If the Windows search feature is not working, run the following PowerShell command and then reboot:

```powershell
Get-AppxPackage MicrosoftWindows.Client.CBS | Reset-AppxPackage
```

---

## Git — common issues & fixes 🧰

### 1) Git not found (PATH)
If Git commands are not recognized, check that Git is installed and that its `cmd` folder is on your PATH.

- Typical path to add (verify on your PC): `C:\Program Files\Git\cmd`
- After adding to PATH, open a new terminal and verify with:

```bash
git --version
```

If you don't have Git installed, download and install it from https://git-scm.com/.

### 2) Git identity (user name & email)
If your Git identity is not set, configure it globally so your commits are attributed correctly:

```bash
# Replace the placeholders with your info
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

Example (replace with your details):

```bash
git config --global user.email "neibaur.isaac@gmail.com"
git config --global user.name "Isaac Neibaur"
```

---

> Tip: After making changes, restart your terminal to ensure environment variable updates are applied.

