# Raspberry Pi Setup

主要拿來放一些設定

# Requirements

- 64-bit OS
  - Bluetooth keyboard & mouse
- Dot files
- Git
- VS code
  - Plugins/extensions?
- Rust
- Python 3
- YubiKey

```
# install vim
sudo apt-get install -y vim

# remap capslock to ctrl
sudo bash -c 'cat << EOF > /etc/default/keyboard
XKBMODEL="macbook78"
XKBLAYOUT="us"
XKBVARIANT=
XKBOPTIONS="ctrl:nocaps"
BACKSPACE="guess"
EOF'
sudo dpkg-reconfigure keyboard-configuration

# install vscode
sudo sh <( wget -O - https://code.headmelted.com/installers/apt.sh )

# install dotfiles
git clone https://github.com/suitingtseng/dotfiles.git ~/dotfiles
mv ~/dotfiles/.gitconfig ~/
mv ~/dotfiles/.bashrc ~/
mv ~/dotfiles/.profile ~/

# install rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

```
