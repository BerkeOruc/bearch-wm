# Bearch-WM

BerkeOS Wayland Compositor based on Hyprland.

## Features

- Wayland compositor with Hyprland
- Beautiful blur and transparency effects
- Custom keybindings for workflow efficiency
- Floating window support for utilities
- Workspace-based window management

## Installation

### Prerequisites

```bash
pacman -S hyprland waybar wofi picom dunst network-manager-applet blueman volumeicon clipman xss-lock xautolock brightnessctl grim playerctl wpctl
```

### Setup

1. Copy the configuration files:

```bash
mkdir -p ~/.config/hypr
cp config/hyprland.conf ~/.config/hypr/
cp config/autostart ~/.config/hypr/
cp config/keybindings.conf ~/.config/hypr/
chmod +x ~/.config/hypr/autostart
```

2. Install the desktop entry:

```bash
cp bearch-wm.desktop ~/.local/share/xsessions/
```

3. Configure your shell (see besrh-shell):

```bash
cp -r ../besrh-shell/* ~/.config/fish/
```

## Configuration

### Keybindings

Keybindings are defined in `config/keybindings.conf`.

| Key | Action |
|-----|--------|
| Super + Enter | Open terminal |
| Super + D | App launcher |
| Super + Q | Close window |
| Super + M | Exit session |
| Super + 1-0 | Switch workspace |
| Super + Shift + 1-0 | Move window to workspace |
| Super + S | Toggle scratchpad |
| Super + L | Lock screen |
| Print | Screenshot |
| Super + Shift + R | Reload config |

### Window Rules

Floating windows:
- pavucontrol
- nm-connection-editor
- blueman-manager

## Autostart

The autostart script launches:
- Waybar (status bar)
- Picom (compositor)
- Dunst (notifications)
- System applets (network, bluetooth, volume)
- Clipman (clipboard)
- Screen locker

## Troubleshooting

### No wallpaper
Install a wallpaper setter or adjust autostart script.

### No transparency
Ensure picom is running and check its configuration.

### Keybindings not working
Check Hyprland logs: `journalctl -xe -u hyprland`

## License

MIT
