# BearchWM - Caelestia Fork for Bearch Linux

BearchWM is a fork of Caelestia customized for Bearch Linux, an Arch-based distribution for developers.

## Description

This is the main repo of the BearchWM dots and contains user configs for apps. Based on Caelestia with Bearch Linux customizations.

## Installation

Simply clone this repo and run the install script (you need [`fish`](https://github.com/fish-shell/fish-shell) installed).

```sh
git clone https://github.com/BerkeOruc/bearch-wm.git ~/.local/share/bearch-wm
~/.local/share/bearch-wm/install.fish
```

### Manual Installation

Dependencies:
- hyprland
- xdg-desktop-portal-hyprland
- xdg-desktop-portal-gtk
- hyprpicker
- wl-clipclip
- cliphist
- inotify-tools
- wireplumber
- trash-cli
- foot
- fish
- fastfetch
- starship
- btop
- jq
- eza

Then copy or symlink the `hypr`, `foot`, `fish`, `fastfetch`, `uwsm` and `btop` folders to `$XDG_CONFIG_HOME` (usually `~/.config`).

## Bearch Tools

This repo includes configurations for Bearch Linux tools:

- **bearch-install** - TUI Installer
- **bearch-aur** - AUR Client (BEAUR)
- **besrh-shell** - Fish Shell Extensions
- **berke-wifi** - WiFi Manager (coming soon)
- **berke-fetch** - System Info Tool (coming soon)

## Keybinds

- `Super` - open launcher
- `Super` + `#` - switch to workspace `#`
- `Super` + `T` - open terminal (foot)
- `Super` + `W` - open browser
- `Super` + `C` - open IDE

## License

GPL-3.0
