

# AurUtil

A simple (bash script) tool to use ArchLinux's Github AUR Mirror instead of the main AUR (aur.archlinux.org)

I make it behave option like pacman and yay btw.

## Installation

This command will put it in ~/.local/bin or will create the folder it if it doesn't exist, then it will download the script into it and and make it executable. (In one command) support both bash and zsh

    mkdir ~/.local/bin; curl -fsSL https://github.com/cltq/aurutil/raw/refs/heads/main/aurutil > ~/.local/bin/aurutil; chmod +x ~/.local/bin/aurutil; echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.zshrc; echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc & source .zshrc & source .bashrc

## Usage

aurutil -S <package> - Install package

 aurutil -R <package> - Remove package
 
 aurutil -Rns <package> - Remove package with deps and configs
 
 aurutil -Syu - Full System + AUR upgrade

 aurutil -Ss <keyword> - Search packages

