# Lanexa APT Repository

APT package repository for Lanexa tools, hosted via GitHub Pages.

## Setup

```bash
# Add the GPG key
curl -fsSL https://lanexadev.github.io/apt/gpg.key | sudo gpg --dearmor -o /usr/share/keyrings/lanexadev.gpg

# Add the repository
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/lanexadev.gpg] https://lanexadev.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/lanexadev.list

# Install
sudo apt update
sudo apt install muxtop
```

## Available packages

- **muxtop** — A modern, multiplexed system monitor for the terminal
