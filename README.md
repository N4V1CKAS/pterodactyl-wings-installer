# 🐉 Pterodactyl + Wings Easy Installer
An interactive Bash script to automate the installation of Pterodactyl Panel and Wings daemon on Ubuntu, saving hours of manual setup.

## 🛠️ Technologies
- Bash scripting
- Core Linux tools and package managers `apt, curl, systemd`

## 🚀 Features
- Interactive menu to choose Panel or Wings installation
- Automatic dependency installation
- MariaDB database setup (Panel)
- Pterodactyl Panel configuration, crontab and queue workers
- Safe checks and user prompts throughout

## 💡 Why I built it
This was my first deep dive into Bash scripting and a practical way to automate a real-world server task I repeat:
- Learning how Bash works in real server setups
- Building an interactive menu that's easy to follow
- Installing dependencies and configuring services step by step
- Testing everything on fresh VMs to fix issues as they came up

## ⚠️ Requirements & Notes
- Ubuntu Server 24.04 (tested, may work on earlier versions)
- Fresh VM/VPS recommended
- User with sudo privileges required
- Wings will **not** start until a valid `config.yml` is placed at `/etc/pterodactyl/`

> Note: This was my first Bash script, built through trial, error and testing on fresh VMs. A small portion (initial menu and password generation) was assisted by AI, however the rest was implemented by reading official documentation and fixing issues as they appeared.

## 📦 Usage
1. Clone the repository
2. Make the script executable: `chmod +x installer.sh`
3. Run the script: `sudo ./installer.sh`
4. Follow the interactive menu
