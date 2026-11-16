# Installing-wsl-as-windows-subsystem-
# 🐧 WSL, Linux and Bash Notes

My notes and practice scripts from learning Linux and Bash on **Windows with WSL 2 and Ubuntu**.

## ⚙️ Setup (WSL + Ubuntu)

Run in PowerShell as Administrator:

```powershell
wsl --install
```

Restart the PC, create a username and password in Ubuntu, then update:

```bash
sudo apt update && sudo apt upgrade -y
```

Check the version:

```powershell
wsl -l -v
```

## 📁 Basic Linux Commands

| Command | What it does |
|---------|--------------|
| `pwd` | Show current folder |
| `ls -la` | List all files with details |
| `cd folder` | Go into a folder |
| `mkdir name` | Create a folder |
| `touch file.txt` | Create an empty file |
| `cp a b` | Copy a file |
| `mv a b` | Move or rename a file |
| `rm file` | Delete a file |
| `cat file` | Show file contents |
| `grep "text" file` | Search inside a file |
| `chmod +x script.sh` | Make a script executable |
| `sudo` | Run as administrator |

## 📜 Bash Scripting Basics

```bash
#!/bin/bash

# Variables
name="DevOps"
echo "Hello, $name!"

# If statement
if [ -f "file.txt" ]; then
  echo "File exists"
else
  echo "File not found"
fi

# Loop
for i in 1 2 3; do
  echo "Number $i"
done
```

Run a script:

```bash
chmod +x script.sh
./script.sh
```

## 🧪 Practice Scripts

| Script | Description |
|--------|-------------|
| `backup.sh` | Back up a folder with a date in the name |
| `health-check.sh` | Show disk, memory, and CPU usage |
| `cleanup-logs.sh` | Delete old log files |

## 🔗 Useful Tips

- Windows files are at `/mnt/c/`
- Open the current folder in VS Code with `code .`
- Use `man command` to read a command's manual

## ✅ What I Learned

- [x] Installed WSL 2 and Ubuntu
- [x] Navigated the file system
- [ ] Wrote my first Bash script
- [ ] Automated a task with cron
