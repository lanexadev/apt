# Lanexa APT Repository

APT package repository for Lanexa tools, hosted via GitHub Pages.

## Setup

```bash
# Add the GPG key
curl -fsSL https://lucasschimmel.github.io/apt/gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/lucasschimmel.gpg

# Add the repository
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/lucasschimmel.gpg] https://lucasschimmel.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/lucasschimmel.list

# Install
sudo apt update
sudo apt install muxtop
```

## Available packages

- **muxtop** — A modern, multiplexed system monitor for the terminal
