# Discord Updater

A lightweight tool that automatically downloads and installs the latest version of **Discord** on Debian/Ubuntu-based Linux distributions (including Linux Mint).  
No more manual `.deb` downloads — keep Discord up-to-date with a single command.



## Features

Always fetches the latest Discord `.deb` package
Installs or updates Discord automatically
Works on **Ubuntu, Linux Mint, Pop!_OS, Debian**, and derivatives
Can be installed via a signed **APT repository**
Updates with sudo apt update.


## Installation

### Add the repository
```
curl -fsSL https://bobbycomet.github.io/Discordupdater/key.gpg | sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/discord-updater.gpg

echo "deb [arch=amd64 signed-by=/etc/apt/trusted.gpg.d/discord-updater.gpg] https://bobbycomet.github.io/Discordupdater/apt noble main" | sudo tee /etc/apt/sources.list.d/discord-updater.list
sudo apt update
```

```
sudo apt install discord-updater
```

```
discord-updater
```

This project is licensed under the MIT License.
Discord itself is a trademark of Discord Inc. This project is not affiliated with or endorsed by Discord.
