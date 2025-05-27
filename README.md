# Hyprland Dotfiles

> # I am currently using [ML4W dotfiles](https://github.com/mylinuxforwork/dotfiles), so it won't be updated for a while

> **Note:** This repository is currently under development and may not be stable. I am actively pushing new configurations and features. Stable releases will be tagged and announced once they are ready. Use at your own discretion if you need a production-ready setup.

Welcome to my Hyprland dotfiles repository! This repository contains detailed configuration files for Hyprland and related applications, organized under the `.config/` directory for easy management and portability.

---

## Table of Contents

- [About Hyprland](#about-hyprland)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

---

## About Hyprland

[Hyprland](https://github.com/hyprwm/Hyprland) is a dynamic tiling Wayland compositor, offering advanced window management, beautiful animations, and extensive customization. It is designed for users who want a fast, modern, and highly configurable desktop experience.

## Repository Structure

All configuration files are stored in their respective directories under `.config/`, following the XDG Base Directory Specification. This makes it easy to manage, back up, and deploy your entire desktop environment.

Example structure:

```
.config/
├── hypr/        # Hyprland main configuration
├── waybar/      # Waybar (status bar) configuration
├── rofi/        # Rofi (launcher) configuration
├── kitty/       # Kitty terminal configuration
├── swaync/      # Sway notification center config
└── ...          # Other application configs
```

> **Note:** Only the configuration directories you use will be present. Add or remove as needed for your setup.

## Getting Started

### Prerequisites

- A Linux distribution with [Hyprland](https://wiki.hyprland.org/Getting-Started/) installed.
- Familiarity with the Linux command line.

### Cloning the Repository

Clone this repository to your home directory:

```bash
git clone https://github.com/yourusername/hyprland-dots.git
cd hyprland-dots
```

### Applying the Dotfiles

1. **Backup your existing configs:**
   ```bash
   cp -r ~/.config ~/.config.backup.$(date +%Y%m%d)
   ```
2. **Copy the configs:**
   ```bash
   cp -r .config/* ~/.config/
   ```
3. **Restart Hyprland:**
   Log out and log back in, or restart Hyprland to apply the new configuration.

## Usage

- **Edit configs:** Tweak files in `.config/{application}` to customize your environment.
- **Add new configs:** Place new application configs under `.config/` to version control them.
- **Keep it portable:** Manage all your desktop settings in one place for easy migration.

## Customization

- **Themes:** Change wallpapers, color schemes, and bar styles in their respective config files.
- **Keybindings:** Adjust keybindings in `.config/hypr/hyprland.conf` and other relevant configs.
- **Integrate tools:** Add configs for other tools (e.g., `dunst`, `mako`, `alacritty`) under `.config/` as needed.

## Contributing

Contributions are welcome! Open issues or submit pull requests to improve these dotfiles or add new features.

## License

This repository is licensed under the [MIT License](LICENSE).

---

**Enjoy your Hyprland experience!**
