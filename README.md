# Hytale Minecraft-Like Controls

> Make Hytale feel like Minecraft with familiar keybindings that ease the transition for Minecraft players.

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## Features

- Complete Minecraft-style control mapping
- Simple installation process
- Fully customizable keybindings
- Optimized graphics and audio settings included

## Installation

### 1. Find Your Settings File

**Windows:**
```
%appdata%\Hytale\install\release\package\game\latest\settings.json
```

**Linux:**
```
~/.local/share/Hytale/install/release/package/game/latest/settings.json
```

**macOS:**
```
~/Library/Application Support/Hytale/install/release/package/game/latest/settings.json
```

### 2. Backup & Install

1. Backup your current `settings.json`
2. Download `Settings.json` from this repository
3. Replace your existing file
4. Launch Hytale

## Controls Overview

| Action | Key | Action | Key |
|--------|-----|--------|-----|
| Move | WASD | Jump | Space |
| Sprint | Left Ctrl | Crouch | Left Shift |
| Inventory | E | Drop Item | Q |
| Chat | T | Map | M |
| Hotbar | 1-9 | Camera | F5 |

## Customize Controls

Edit the `InputBindings` section in `settings.json`:

```json
"Jump": {
  "Key": 32
},
"Crouch": {
  "Scancode": 225
}
```

### Common Key Codes
- Space: `{"Key": 32}`
- Left Shift: `{"Scancode": 225}`
- Left Ctrl: `{"Scancode": 224}`
- E: `{"Scancode": 8}`
- Q: `{"Scancode": 20}`

## Troubleshooting

**Controls not working?**
- Verify file location
- Restart Hytale completely
- Check file isn't read-only

**Performance issues?**
- Lower `RenderScale` (default: 75%)
- Reduce `ViewDistance`
- Disable visual effects in settings

**Want to revert?**
- Use your backup or delete `settings.json` to regenerate defaults

## Contributing

Contributions welcome! Fork the repo, make your changes, and submit a pull request.

## License

MIT License - see [LICENSE](LICENSE) for details.

## Credits

Created for the Hytale community by Minecraft players. Not affiliated with Hytale or Mojang Studios.

---

⭐ **Star this repo if it helped you!**
