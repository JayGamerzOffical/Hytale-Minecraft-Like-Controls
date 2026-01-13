# 🎮 Hytale Minecraft-Like Controls

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Downloads](https://img.shields.io/github/downloads/JayGamerzOffical/Hytale-Minecraft-Like-Controls/total.svg)]()
[![Stars](https://img.shields.io/github/stars/JayGamerzOffical/Hytale-Minecraft-Like-Controls.svg)]()
[![Issues](https://img.shields.io/github/issuesJayGamerzOffical/Hytale-Minecraft-Like-Controls.svg)]()

> Transform your Hytale experience with familiar Minecraft controls! This configuration file modifies Hytale's default keybindings to match Minecraft's control scheme, making the transition seamless for Minecraft players.

## 📋 Table of Contents

- [✨ Features](#-features)
- [📦 Installation](#-installation)
- [🎯 Usage](#-usage)
- [⚙️ Customization](#️-customization)
- [🎮 InputBindings Only](#-inputbindings-only)
- [❓ Troubleshooting](#-troubleshooting)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🙏 Credits](#-credits)

## ✨ Features

- **🎯 Minecraft-Style Controls**: All essential controls mapped to match Minecraft's layout
- **⚡ Quick Setup**: Simple copy-paste installation process
- **🔧 Customizable**: Easy to modify individual keybindings
- **📱 Complete Coverage**: Movement, combat, inventory, and building tools
- **🔄 Backup Friendly**: Non-destructive installation with backup instructions
- **🎨 Optimized Settings**: Includes optimized graphics and audio settings

### What's Included

- Complete `settings.json` with Minecraft-like controls
- Optimized display and performance settings
- Builder tools configuration
- Audio and mouse sensitivity presets
- Input behavior settings for smooth gameplay

## 📦 Installation

### Step 1: Locate Your Hytale Settings Directory

Navigate to your Hytale settings folder:
```
%APPDATA%\Hytale\
```
or
```
C:\Users\[YourUsername]\AppData\Roaming\Hytale\
```

### Step 2: Backup Your Current Settings

Before installing, backup your existing configuration:
```bash
copy settings.json settings_backup.json
```

### Step 3: Install the New Configuration

1. Download the `Settings.json` file from this repository
2. Replace your existing `settings.json` with the downloaded file
3. Launch Hytale to apply the new controls

## 🎯 Usage

Once installed, you'll immediately notice the familiar Minecraft control scheme:

### Basic Movement
- **W** - Move Forward
- **A** - Strafe Left  
- **S** - Move Backward
- **D** - Strafe Right
- **Space** - Jump/Fly Up
- **Left Shift** - Crouch/Fly Down
- **Left Ctrl** - Sprint

### Combat & Interaction
- **Left Click** - Primary Attack (Break blocks)
- **Right Click** - Secondary Action (Place blocks/Use items)
- **Middle Click** - Pick Block
- **E** - Open Inventory
- **Q** - Drop Item

### Hotbar
- **1-9** - Select Hotbar Slots
- **F** - Switch Utility Slot

### Navigation & UI
- **T** - Chat
- **Tab** - Show Player List
- **M** - Open Map
- **B** - Open Tools Settings
- **C** - Activate Camera Rotation
- **F5** - Switch Camera Mode

## ⚙️ Customization

### Modifying Individual Controls

1. Open `settings.json` in a text editor
2. Navigate to the `InputBindings` section
3. Find the action you want to modify
4. Change the key code (see Key Codes section below)

### Key Codes Reference

| Action | Key Code | Description |
|--------|----------|-------------|
| Space | `{"Key": 32}` | Jump/Fly Up |
| Left Shift | `{"Scancode": 225}` | Crouch/Sneak |
| Left Ctrl | `{"Scancode": 224}` | Sprint |
| E | `{"Scancode": 8}` | Inventory |
| Q | `{"Scancode": 20}` | Drop Item |

### Graphics Settings

The configuration includes optimized settings:
- **Render Scale**: 75% (balanced performance)
- **View Distance**: 192 chunks
- **Anti-Aliasing**: FXAA
- **FPS Limit**: 240 FPS
- **VSync**: Enabled

## 🎮 InputBindings Only

If you want to keep your existing settings and only change the controls, use this standalone `InputBindings` configuration:

### How to Merge InputBindings

1. Open your current `settings.json`
2. Find the `InputBindings` section (around line 40)
3. Replace the entire section with the code below
4. Save and restart Hytale

```json
"InputBindings": {
  "MoveForwards": {
    "Scancode": 26
  },
  "MoveBackwards": {
    "Scancode": 22
  },
  "StrafeLeft": {
    "Scancode": 4
  },
  "StrafeRight": {
    "Scancode": 7
  },
  "Jump": {
    "Key": 32
  },
  "Crouch": {
    "Scancode": 225
  },
  "Sprint": {
    "Scancode": 224
  },
  "Walk": {
    "Key": 1073742050
  },
  "FlyUp": {
    "Key": 32
  },
  "FlyDown": {
    "Scancode": 225
  },
  "PrimaryItemAction": {
    "MouseButton": 1
  },
  "SecondaryItemAction": {
    "MouseButton": 3
  },
  "Ability1ItemAction": {
    "Scancode": 29
  },
  "Ability2ItemAction": {
    "Scancode": 8
  },
  "Ability3ItemAction": {
    "Scancode": 21
  },
  "BlockInteractAction": {
    "Scancode": 9
  },
  "RotateBlock": {
    "Key": 114
  },
  "ShowUtilitySlotSelector": {
    "Scancode": 29
  },
  "DismountAction": {
    "Scancode": 9
  },
  "DropItem": {
    "Scancode": 20
  },
  "HotbarSlot1": {
    "Key": 49
  },
  "HotbarSlot2": {
    "Key": 50
  },
  "HotbarSlot3": {
    "Key": 51
  },
  "HotbarSlot4": {
    "Key": 52
  },
  "HotbarSlot5": {
    "Key": 53
  },
  "HotbarSlot6": {
    "Key": 54
  },
  "HotbarSlot7": {
    "Key": 55
  },
  "HotbarSlot8": {
    "Key": 56
  },
  "HotbarSlot9": {
    "Key": 57
  },
  "SwitchCameraMode": {
    "Scancode": 62
  },
  "ActivateCameraRotation": {
    "Key": 99
  },
  "Chat": {
    "Scancode": 23
  },
  "PickBlock": {
    "MouseButton": 2
  },
  "SwitchGameMode": {
    "Scancode": 60
  },
  "OpenInventory": {
    "Scancode": 8
  },
  "OpenMachinimaEditor": {
    "Scancode": 17
  },
  "OpenMap": {
    "Key": 109
  },
  "OpenToolsSettings": {
    "Key": 98
  },
  "OpenDevTools": {
    "Scancode": 53
  },
  "ShowPlayerList": {
    "Key": 112
  },
  "ToggleBuilderToolsLegend": {
    "Key": 108
  },
  "PreviousBuilderToolsLegendPage": {
    "Key": 106
  },
  "NextBuilderToolsLegendPage": {
    "Key": 107
  },
  "UndoItemAction": {
    "Key": 122
  },
  "RedoItemAction": {
    "Key": 121
  },
  "AddRemoveFavoriteMaterialItemAction": {
    "Key": 0
  },
  "ToolPaintBrush": {
    "Key": 1073741913
  },
  "ToolSculptBrush": {
    "Key": 1073741914
  },
  "ToolSelectionTool": {
    "Key": 1073741915
  },
  "ToolPaste": {
    "Key": 1073741916
  },
  "ToolLine": {
    "Key": 1073741917
  },
  "AlternatePlaySculptBrushModeModifier": {
    "Key": 1073742049
  },
  "UsePaintModeForBrush": {
    "Key": 117
  },
  "SelectBlockFromSet": {
    "Scancode": 20
  },
  "PastePreview": {
    "Key": 116
  },
  "SwitchHudVisibility": {
    "Key": 1073741889,
    "Modifiers": 0
  },
  "ToggleFullscreen": {
    "Key": 1073741892
  },
  "TakeScreenshot": {
    "Key": 1073741893
  },
  "Command": {
    "Scancode": 56
  },
  "DecreaseSpeedMultiplier": {
    "Key": 1073741882
  },
  "IncreaseSpeedMultiplier": {
    "Key": 1073741883
  },
  "ToggleCreativeCollision": {
    "Key": 1073741884
  },
  "ToggleFlyCamera": {
    "Key": 1073741885
  },
  "ToggleFlyCameraControlTarget": {
    "Key": 1073741886
  },
  "ToggleDebugScreens": {
    "Key": 1073741888
  },
  "CrouchInputBehavior": 0,
  "SprintInputBehavior": 0,
  "WalkInputBehavior": 0
}
```

## ❓ Troubleshooting

### Common Issues

**Q: Controls aren't working after installation**
- Make sure you've placed the `settings.json` in the correct directory
- Restart Hytale completely after installing
- Check that the file isn't set to read-only

**Q: Some keys feel different from Minecraft**
- This configuration uses Hytale's input system, so some actions may have slight variations
- Check the InputBindings section above for exact mappings

**Q: Game crashes after installing**
- Restore your backup (`settings_backup.json`)
- Verify the JSON file is valid (no syntax errors)
- Ensure FormatVersion matches your Hytale version

**Q: I want to revert to default controls**
- Use your backup file or delete `settings.json` to regenerate defaults

### Performance Issues

If you experience performance problems:
- Lower `RenderScale` in RenderingSettings
- Reduce `ViewDistance` 
- Disable some visual effects like `Bloom` or `DepthOfField`

## 🤝 Contributing

We welcome contributions to improve this Hytale control configuration!

### How to Contribute

1. **Fork** this repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Contribution Guidelines

- Test your changes thoroughly before submitting
- Maintain the existing code style and formatting
- Update documentation if you add new features
- Ensure all JSON syntax is valid

### Areas for Improvement

- [ ] Additional control schemes (FPS, Builder, etc.)
- [ ] Performance presets for different hardware
- [ ] Localization support
- [ ] Auto-installation script

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 Hytale Minecraft Controls

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 🙏 Credits

- **Hytale Development Team** - For creating this amazing game
- **Minecraft Community** - For inspiring these intuitive controls
- **Contributors** - Everyone who helps improve this configuration

### Special Thanks

- Thank you to the Hytale beta testers for feedback
- Appreciation to the Minecraft veterans who suggested improvements
- Recognition of the modding community for inspiration

---

## 🌟 Show Your Support

If this configuration helped you transition to Hytale, please consider:

- ⭐ **Star** this repository
- 🐛 **Report** any issues you encounter
- 💡 **Suggest** improvements and new features
- 🔄 **Share** with other Minecraft players

**Enjoy your seamless Hytale experience with familiar Minecraft controls! 🎮✨**

---

*This project is not affiliated with or endorsed by Hytale or Mojang Studios. All trademarks belong to their respective owners.*
