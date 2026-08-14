# Staticaliza's Blender Animation Tools for Roblox

<p align="center">
  <img src="docs/logo.png" alt="Staticaliza's Blender Animation Tools">
</p>

One Blender extension provides three focused N-panels:

- **Roblox Animator** — Cautioned's importer, rigging, animation, and export workflow.
- **Roblox Animator Utils** — Staticaliza's animation, contact-pin, ragdoll, camera, onion-skin, and rig utilities.
- **Roblox Animator Impact** — Staticaliza's anime impact-frame authoring and preview renderer.

Blender Preferences shows one entry, **Staticaliza's Blender Animation Tools**. Roblox Animator, Utils, and Impact are private modules inside that extension and retain separate N-panel tabs.

The complete toolset supports **Blender 4.2 through Blender 5.2**. Most animation tools are intended for Pose Mode.

## Current Versions

- **Roblox Animator Utils:** 1.7.0
- **Roblox Animator Impact:** 1.0.0
- **Extension Setup:** 1.0.0

The unified extension registers Roblox Animator first, Roblox Animator Utils second, and Roblox Animator Impact third.

## Installation

1. Download `staticaliza_blender_animation_tools.zip` from the [latest GitHub release](https://github.com/Staticaliza/Staticaliza-Blender-Animation-Tools/releases/latest).
2. In Blender, open **Edit > Preferences > Get Extensions**.
3. Choose **Install from Disk** and select the ZIP.
4. Enable **Staticaliza's Blender Animation Tools** if Blender does not enable it automatically. No child extensions need to be installed separately.

To update later, open **Roblox Animator Utils > Extension** and choose the update action. It replaces the single unified extension; Impact has no separate in-panel updater.

The **Install Roblox Plugins** button opens the recommended [Roblox Blender Animation Tools](https://create.roblox.com/store/asset/118148792788940) and [companion animation plugin](https://create.roblox.com/store/asset/16708835782).

## Features

- **Animation Tools**: Dynamic Parent, Dynamic Unparent, Surface Contact, ragdoll, and camera tools.
- **Active Armatures**: Work with multiple rigs in Pose Mode while inactive rigs stay visually separated.
- **Rig Cleanup**: Remove imported rigs with one undoable action while preserving shared assets.
- **Onion Tools**: Preview meshes and bones with selectable Onion Pins, Contact targets, and snap rings.
- **Surface Contact**: Create and animate contacts with collision, sliding, tracking, and IK support.
- **Impact Frames**: Author and preview impact-frame looks in the dedicated Roblox Animator Impact N-panel.
- **Viewport Workflow**: Synchronize viewport and animation-editor settings across workspaces.
- **Camera Tools**: Attach adjustable-FOV cameras to selected bones and keyframe camera views.
- **Export**: Export dense relationship, contact, and layered animation data.

## Shortcuts

| Shortcut | Action |
| --- | --- |
| `Tab` | Toggle animation loop |
| `F` | Toggle Onion Skin |
| `Shift + F` | Create or manage Onion Pins |
| `Ctrl + F` | Open Animation Tools |
| `Y` | Switch Global/Local orientation |
| `Shift + Y` | Switch Bone/Object pivot |

## Advanced Mode

Advanced Mode is disabled by default. Enabling it exposes Materials, Miscellaneous, detailed Onion settings, material processing, Surface Contact filtering, manual Bake controls, rig-generation controls, helper visibility, and Roblox Animator's advanced panels.

## Release File

GitHub Releases contains one unified extension archive:

| File | Purpose |
| --- | --- |
| GitHub Release asset: `staticaliza_blender_animation_tools.zip` | One installed extension containing Roblox Animator, Utils, and Impact |

## Author

This project and its releases are authored by **Staticaliza** (`413584@gmail.com`).

## Credits

- [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin)
- **Dynamic Parent 2.0.2** by Roman Volodin, updated for Blender 4.2 through 5.2 and Roblox animation export.

## License

Roblox Animator Utils and Roblox Animator Impact are distributed under the GNU General Public License v2.0 or later.
