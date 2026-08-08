# Staticaliza's Blender Animation Tools for Roblox

<p align="center">
  <img src="docs/logo.png" alt="Staticaliza's Blender Animation Tools">
</p>

Staticaliza's Blender Animation Tools installs [Cautioned's Roblox Animator](https://github.com/Cautioned/Blender-Animations-Plugin) and adds the **Roblox Animator Utils** workflow for importing, preparing, animating, and exporting Roblox rigs.

The complete toolset supports **Blender 4.2 through Blender 5.2**. Most animation tools are intended for Pose Mode.

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

- **Animation Tools**: Dynamic Parent, Dynamic Unparent, Surface Contact, and camera tools.
- **Active Armatures**: Work with multiple rigs in Pose Mode while inactive rigs stay visually separated.
- **Rig Cleanup**: Remove imported rigs with one undoable action while preserving shared assets.
- **Multi-Rig Feedback**: Keep same-named bones tied to the correct rig with clear rig labels.
- **Onion Tools**: Preview meshes and bones with selectable Onion Pins, Contact targets, and snap rings.
- **Pin Transforms**: Select and transform pins independently or with bones using `G`, `R`, and `S`.
- **Surface Contact**: Create and animate contacts with collision, sliding, tracking, and IK support.
- **State Feedback**: Show relationship and contact states with ordered action channels and status labels.
- **Impact Frames**: Shared impact-frame markers are planned for an upcoming release.
- **Viewport Workflow**: Synchronize viewport and animation-editor settings across workspaces.
- **Camera Tools**: Attach adjustable FOV cameras to selected bones and keyframe camera views.
- **Rig Setup**: Prepare imported rigs with Pose Mode, channel organization, constraints, and helper controls.
- **Materials**: Import and isolate materials while standardizing viewport appearance.
- **Export**: Export dense relationship and contact animation with partial-body layering support.
- **Scene Setup**: Load the bundled template, texture, layout, and viewport settings.

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

Contributor and release instructions are in [CONTRIBUTING.md](CONTRIBUTING.md).

## Author

This project and its releases are authored by **Staticaliza** (`413584@gmail.com`).

## Credits

- [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin)
- **Dynamic Parent 2.0.2** by Roman Volodin, updated for Blender 4.2 through 5.2 and Roblox animation export.

## License

Roblox Animator Utils is distributed under the GNU General Public License v2.0 or later.
