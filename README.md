# Unity Tilemap Prefab Placer

A free Unity Editor tool for placing prefabs on a grid with precision. Perfect for level design, tile-based games, and any project requiring grid-aligned object placement.

![Unity Version](https://img.shields.io/badge/Unity-6000.0%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)


## ✨ Features

- 🎯 Grid-snapped placement with visual feedback
- 🎨 Multi-prefab palette with sprite previews
- ⌨️ Keyboard shortcuts (0-9) for quick prefab switching
- 📐 Pivot offset support for perfect alignment
- ↩️ Full undo/redo support
- 🗂️ Automatic hierarchy organization

![tilemap-prefab-placer-video](https://github.com/user-attachments/assets/e647d3d4-3543-43dd-afa9-8beae7efc9be)


## 📦 Installation

### Unity Package Manager (Recommended)
1. Open Package Manager (`Window > Package Manager`)
2. Click `+` → `Add package from git URL`
3. Enter: `https://github.com/berkanozgur/Tilemap-Prefab-Placer.git`

### Manual Installation
Sample project made in Unity 6, but it should work fine in previous versions.

1. Download the latest release
2. Extract to a folder
3. Open in Unity Hub
4. Access via `Tools > Tilemap Prefab Placer`

or

Copy "Tilemap Prefab Placer" folder into your project.

or

Copy "TilemapObjectPlacer.cs" into any "Editor" folder (must be in a folder named "Editor").

## 📖 Quick Start

### 1. Open the Tool
**Tools → Tilemap Prefab Placer**

### 2. Assign Your Grid
Drag your Grid component into the tool panel.

<img width="789" height="323" alt="image" src="https://github.com/user-attachments/assets/c497bcd3-ab6c-4885-9cda-dceb2ac424e2" />


### 3. Select Prefabs

**Single Prefab Mode:**

**Multiple Prefabs (Palette Mode):**
- Click "+ Add Prefab Slot"
- Assign prefabs to slots
- Click checkbox to select active prefab
- Selected prefab shows with yellow background

<img width="505" height="718" alt="image" src="https://github.com/user-attachments/assets/869f97a3-b8e8-40ed-9ee3-e5db568f20d8" />

### 4. Enable Place Mode
Toggle "Place Mode" button (turns green when active).

<img width="434" height="411" alt="image" src="https://github.com/user-attachments/assets/54ae6f8e-44e0-419b-9ce3-3762d928d646" />

### 5. Place Objects
Visual gizmos show placement position and grid coordinates.

<img width="445" height="454" alt="image" src="https://github.com/user-attachments/assets/93814650-90ec-4fee-bc0a-4952dcafa902" />

## ⌨️ Controls

| Action | Shortcut |
|--------|----------|
| Place object | `Shift + Click` |
| Remove object | `Ctrl + Shift + Click` |
| Select prefab | `0-9` keys |
| Disable temporarily | Hold `Alt` |

## ⚙️ Settings

**Parent Object Name**
- Organizes placed objects under a parent GameObject
- Default: "PlacedObjects"

**Pivot Offset**
- Adjust placement position for non-centered sprites
- Example: `(0, -0.5, 0)` for bottom-aligned sprites

**Show Prefab Previews**
- Toggle sprite previews in palette

**Show Grid Gizmos**
- Toggle visual indicators in Scene view

## 📐 Scene Organization
```
Grid
├── Tilemap
└── PlacedObjects (auto-created)
    ├── Prefab(Clone)
    ├── Prefab(Clone)
    └── ...
```

## ⚠️ Important Notes

- **Sprite Previews**: Prefabs need a SpriteRenderer component (checks root, then children)
- **Object Removal**: Always use `Ctrl + Shift + Click` or "Clear All" button - don't delete from hierarchy directly
- **Refresh**: Use "Refresh Placed Objects" button to rescan scene objects

## 🎮 Sample Scene

Included **"Prefab_Placer_Sample"** scene contains:
- Pre-configured Grid and Tilemap
- Player controller with WASD movement
- Sample prefabs to test placement
- Free art from [OpenGameArt](https://opengameart.org/)

## 📄 License

MIT License - See [LICENSE](LICENSE) file for details.


## 💬 Support

📧 **Email**: [berkan.ozgur2@gmail.com](mailto:berkan.ozgur2@gmail.com)

## 🙏 Credits

- **Created by**: Berkan Özgür
- **Sample Art**: [OpenGameArt](https://opengameart.org/)

---

<p align="center">
  ⭐ Star this repo if it helped your project!
</p>
