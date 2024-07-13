Here's a script to install Go, gopls, Node.js, TypeScript, Rust, Yarn, VLC, Telegram Desktop, Fish, and PHP on Manjaro Linux:

bash

#!/bin/bash

# Update system
sudo pacman -Syu --noconfirm

# Install Go
sudo pacman -S go --noconfirm

# Install gopls (Go language server)
GO111MODULE=on go get golang.org/x/tools/gopls@latest

# Install Node.js and npm
sudo pacman -S nodejs npm --noconfirm

# Install TypeScript
sudo npm install -g typescript

# Install Rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
source $HOME/.cargo/env

# Install Yarn
sudo npm install -g yarn

# Install VLC
sudo pacman -S vlc --noconfirm

# Install Telegram Desktop
sudo pacman -S telegram-desktop --noconfirm

# Install Fish shell
sudo pacman -S fish --noconfirm

# Install PHP
sudo pacman -S php --noconfirm

echo "All specified packages have been installed successfully."

To use this script:

    Save the script to a file, for example, install_packages.sh.
    Make the script executable:

    bash

chmod +x install_packages.sh

Run the script:

bash

./install_packages.sh
