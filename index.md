---
layout: "default"
title: "🖥️ TWM - Easy Setup for Window Management"
description: "⚙️ Simplify your desktop experience with TWM, a unified configuration for Niri, Sway, and i3 window managers, featuring easy setup and seamless updates."
---
# 🖥️ TWM - Easy Setup for Window Management

[![Download TWM](https://img.shields.io/badge/Download-TWM-blue.svg)](https://github.com/Rahul225622/TWM/releases)

## 🚀 Getting Started

TWM is a simple configuration package for the Niri, Sway, and i3 window managers. It helps you set up your desktop environment quickly, letting you focus on your work instead of configuration.

## 📥 Download & Install

To get started, visit this page to download the latest version: [Download TWM](https://github.com/Rahul225622/TWM/releases). You will find the release files there. 

After downloading, follow these steps to install:

1. Open your terminal.
   
2. Create a directory for TWM:
   ```bash
   mkdir -p ~/.config/TWM
   ```

3. Clone the repository:
   ```bash
   git clone https://github.com/iamcheyan/TWM.git ~/.config/TWM
   ```

4. Navigate to the TWM directory:
   ```bash
   cd ~/.config/TWM
   ```

5. Make the initialization script executable:
   ```bash
   chmod +x init.sh
   ```

6. Run the initialization script:
   ```bash
   ./init.sh
   ```

This script backs up your existing configuration and creates the necessary links for your window manager.

## ⚙️ Configuration Details

TWM sets up configurations for Niri, Sway, and i3. The Waybar will automatically load the appropriate settings based on your window manager.

- Niri config: `~/.config/waybar/niri/config.jsonc`
- Sway config: `~/.config/waybar/sway/config.jsonc`

## ⚙️ Dependencies Installation

Depending on the window manager you use, you might need to install some additional tools. 

### 🌌 For Sway (Wayland)

If you're using Sway, you need to install these packages:

#### Debian/Ubuntu
```bash
sudo apt update
sudo apt install -y sway waybar kitty swaybg mako wofi fcitx5 \
  brightnessctl grim slurp wl-clipboard libnotify-bin
```

#### Fedora
```bash
sudo dnf install -y sway waybar kitty swaybg mako wofi fcitx5 \
  brightnessctl grim slurp wl-clipboard libnotify
```

#### Arch
```bash
sudo pacman -S --needed sway waybar kitty swaybg mako wofi fcitx5 \
  brightnessctl grim slurp wl-clipboard libnotify
```

### 🖥️ For i3 (X11)

For users of i3, you need the following packages:

#### Debian/Ubuntu
```bash
sudo apt update
sudo apt install -y i3 waybar kitty dunst fcitx5 \
  brightnessctl grim slurp
```

#### Fedora
```bash
sudo dnf install -y i3 waybar kitty dunst fcitx5 \
  brightnessctl grim slurp
```

#### Arch
```bash
sudo pacman -S --needed i3 waybar kitty dunst fcitx5 \
  brightnessctl grim slurp
```

## 💡 Additional Features

- **Backup and Restore**: The initialization script automatically backs up your existing configurations to prevent data loss.
- **Customizable Options**: Each configuration file can be easily modified to suit your personal preferences.
- **Community Support**: Users can access a community forum for tips and troubleshooting advice.

## 🔄 Updating TWM

To update TWM, repeat the download and installation steps. Run the `init.sh` script again after downloading the latest version. It will overwrite old configurations with the new defaults.

## 📬 Need Help?

If you encounter any issues, please check the issues section on the [GitHub page](https://github.com/Rahul225622/TWM/issues). You can also ask questions or report bugs there.

Thank you for using TWM! Enjoy your window manager setup.