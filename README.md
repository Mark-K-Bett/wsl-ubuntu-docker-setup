# wsl-ubuntu-docker-setup


### Step 1: Enable WSL & Virtualization

- Open `optionalfeatures.exe`
- Enable:
  - Windows Subsystem for Linux
  - Virtual Machine Platform
- Restart your system

### Step 2: Install WSL via PowerShell

Open PowerShell as Administrator and run:

`powershell
wsl --install `


### Step 3: Launch Ubuntu & Configure It

After `wsl --install` finishes, it will launch Ubuntu (or you can open it from Start Menu). On first launch:

- It sets up the distro
- Prompts you to create:
  - **UNIX username**
  - **Password**
 
### Step 4: Update and Upgrade Ubuntu

In the Ubuntu terminal:

```bash
sudo apt update && sudo apt upgrade -y
```

 
 ### Step 5: Confirm WSL Status

Back in **PowerShell**, check the status:
```powershell
wsl --status
```