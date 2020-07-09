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
sudo vim /etc/default/keyboard

XKBOPTIONS="ctrl:nocaps"

sudo dpkg-reconfigure keyboard-configuration

```


