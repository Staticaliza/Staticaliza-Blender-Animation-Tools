# Staticaliza's Blender Animation Tools for Roblox

Staticaliza's Blender Animation Tools installs [Cautioned's Roblox Animator](https://github.com/Cautioned/Blender-Animations-Plugin) and adds the **Roblox Animator Utils** workflow for importing, preparing, animating, and exporting Roblox rigs.

Roblox Animator Utils supports **Blender 4.2 through Blender 5.2**. Most animation tools are intended for Pose Mode.

## Installation

1. Download `Staticaliza's Blender Animation Tools.zip`.
2. In Blender, open **Edit > Preferences > Get Extensions**.
3. Choose **Install from Disk** and select the ZIP.
4. Open **Roblox Animator Utils > Extension** and use **Install Latest Extension** whenever you want to update both extensions.

The lightweight setup extension installs:

- **Roblox Animator**: Cautioned's importer, rigging, animation, and export extension.
- **Roblox Animator Utils**: Staticaliza's animation workflow and utilities.

The **Install Roblox Plugins** button opens the recommended [Roblox Blender Animation Tools](https://create.roblox.com/store/asset/118148792788940) and [companion animation plugin](https://create.roblox.com/store/asset/16708835782).

## Features

- **Animation Tools**: Dynamic Parent, Dynamic Unparent, Surface Contact, and bone-attached cameras under one `Ctrl + F` menu and N-panel group.
- **Onion Tools**: Mesh and bone previews, Smart Pins, pin pivots, connected-object surface placement, and snap rings.
- **Surface Contact**: Collision-safe Smart Pin contacts with blended limb aiming for feet, hands, IK endpoints, floors, walls, slopes, animated surfaces, and visible rig objects.
- **Camera Tools**: Bone-tip cameras, adjustable FOV presets, local-axis orientation, default attached-object hiding, and keyframing that enters camera view.
- **Rig Setup**: Automatic Local Y-axis armatures, matching-part constraints, duplicate-weld prevention, helper-bone hiding, and multi-rig scene detection.
- **Materials**: Smart material import, safe Base Color and Alpha clearing, per-rig texture isolation, viewport standardization, and optional clothing-clipping prevention.
- **Export**: Dynamic relationships and contacts are densely evaluated through Roblox Animator for smooth Roblox playback.
- **Scene Setup**: A standalone panel below Transform Tools that loads the bundled template, packed Baseplate texture, saved UI layout, and viewport shading after warning about unsaved changes.

Export each Roblox rig into its own folder. If Roblox exports overwrite PNG files before Blender imports them, the original texture data cannot be recovered.

## Shortcuts

| Shortcut | Action |
| --- | --- |
| `F` | Toggle Onion Skin |
| `Shift + F` | Create or manage Onion Pins |
| `Ctrl + F` | Open Animation Tools |
| `Y` | Switch Global/Local orientation |
| `Shift + Y` | Switch Bone/Object pivot |

## Advanced Mode

Advanced Mode is disabled by default. Enabling it exposes Materials, Miscellaneous, detailed Onion settings, material processing, Surface Contact filtering, manual Bake controls, rig-generation controls, helper visibility, and Roblox Animator's advanced panels.

## Release Files

| File | Purpose | Upload When |
| --- | --- | --- |
| `Staticaliza's Blender Animation Tools.zip` | Lightweight setup/downloader | Setup code changes |
| `src/staticaliza_blender_animation_tools.zip` | Roblox Animator Utils source payload | Utils code, template, or version changes |

Use `Build Source ZIP.cmd` for Utils-only changes or `Build Setup ZIP.cmd` when the downloader changes.

## Credits

- [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin)
- **Dynamic Parent 2.0.2** by Roman Volodin, updated for Blender 4.2 through 5.2 and Roblox animation export.

## License

Roblox Animator Utils is distributed under the GNU General Public License v2.0 or later.
