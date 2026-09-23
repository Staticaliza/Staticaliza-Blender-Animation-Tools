# Staticaliza's Blender Animation Tools for Roblox

<p align="center">
  <img src="docs/logo.png" alt="Staticaliza's Blender Animation Tools">
</p>

One Blender extension provides three focused N-panels:

- **Roblox Animator** — Cautioned's importer, rigging, animation, and export workflow.
- **Roblox Animator Utils** — Staticaliza's animation, contact-pin, Smart Dragger, ragdoll, camera, onion-skin, and rig tools.
- **Roblox Animator Impact** — Staticaliza's keyed anime impact frames, with subject and background lines, lighting, effects, live preview, and frame export.

Blender Preferences shows one entry, **Staticaliza's Blender Animation Tools**. Its lightweight host downloads Roblox Animator, Utils, and Impact as private runtimes and retains three separate N-panel tabs.

The complete toolset supports **Blender 4.2 through Blender 5.2**. Most animation tools are intended for Pose Mode.

## Current Versions

- **Roblox Animator Utils:** 1.7.0
- **Roblox Animator Impact:** 1.0.0
- **Extension Setup:** 1.0.0

The Setup extension installs the latest Roblox Animator release and the Utils and Impact runtime ZIPs from this repository's `src/`, then registers the three N-panels in that order. `src/` contains the two runtime ZIPs; the installable Setup ZIP is provided on the GitHub release page.

The Setup release is a small installer. When enabled with online access, it fetches the current runtime ZIPs; later fixes to Utils and Impact can arrive without a new Setup version. The Roblox Animator version is selected from its upstream release at install time.

## Installation

1. Download `staticaliza_blender_animation_tools.zip` from the [latest GitHub release](https://github.com/Staticaliza/Staticaliza-Blender-Animation-Tools/releases/latest).
2. In Blender, open **Edit > Preferences > Get Extensions**.
3. Choose **Install from Disk** and select the ZIP.
4. Enable **Staticaliza's Blender Animation Tools** and allow online access. The lightweight host downloads and privately loads all three tools; no child extensions need to be installed separately.

To update later, open **Roblox Animator > Configuration** and choose **Install Latest Extensions**. It downloads and hot-loads the latest Roblox Animator, Utils, and Impact runtimes; Impact has no separate in-panel updater.

The **Install Roblox Plugins** button opens the recommended [Staticaliza's Blender Animation Tools](https://create.roblox.com/store/asset/118148792788940/Staticalizas-Blender-Animation-Tools) and [**Blender Animations (ultimate edition)**](https://create.roblox.com/store/asset/16708835782/Blender-Animations-ultimate-edition).

## Features

- **Animation Tools**: Dynamic Parent, Dynamic Unparent, pink Surface Contact pins, orange ragdoll pins, and keyframe-handle controls. An active ragdoll controls a bone's motion when that bone also has Surface Contact.
- **Armature Tools**: Work with multiple rigs in Pose Mode while inactive rigs stay visually separated, and remove imported rigs with one undoable cleanup action that preserves shared assets.
- **Onion Tools**: Preview meshes and bones with selectable Onion Pins, Contact targets, and snap rings.
- **Camera and Pin Tools**: Attach adjustable-FOV cameras to selected bones, keyframe camera views, switch bone/object pivots, and pose with Smart Draggers.
- **Impact Tools**: Create keyed impact drawings from one or multiple rigs, adjust subject and background linework, lighting, shapes, and effects, then export frames from the dedicated Impact N-panel.
- **Animation Exchange**: Transfer animation and camera data between Roblox Studio and Blender.

## Shortcuts

| Shortcut | Action |
| --- | --- |
| `Tab` | Toggle animation loop |
| `F` | Toggle Onion Skin |
| `Shift + F` | Create or manage Onion Pins |
| `Ctrl + F` | Open Animation Tools |
| `Y` | Switch Global/Local orientation |
| `Shift + Y` | Switch Bone/Object pivot |

## Credits

- Project and releases authored by **Staticaliza**.
- [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin)
- **Dynamic Parent**, integrated with Roblox animation export.

## License

The Setup, Utils, and Impact package manifests declare GNU General Public License v2.0 or later. The repository's [LICENSE](LICENSE) file contains GNU General Public License v3.0 text.
