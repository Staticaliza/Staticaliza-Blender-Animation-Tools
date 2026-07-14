# Staticaliza's Blender Animation Tools for Roblox/Blender

This Blender extension, which currently only supports Blender 4.3.0, adds additional Roblox animation tools and works alongside [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin), which supports importing and animating Roblox rigs in Blender.

It is recommended to install the [Roblox Blender Animation Tools plugin](https://create.roblox.com/store/asset/118148792788940), which allows avatar rigs to be imported into Blender using Cautioned's animation plugin.

## Automatic Setup

Install `Staticaliza's Blender Animation Tools.zip` through Blender's **Install from Disk** option.

The setup extension automatically downloads, installs, and enables the latest versions of:

- **Roblox Animator**: Cautioned's Blender Animations Plugin
- **Roblox Animator Utils**: Staticaliza's Blender Animation Tools

The setup extension displays the installed version of each extension. Downloaded and repackaged temporary files are automatically removed after installation.

## Features

- Onion Skins (`F`)
- Onion Pins (`Shift + F`)
- Unparent with start and end keyframes (`Alt + F`)
- Dynamic Parent with start and end keyframes (`Shift + Alt + F`)
- Smart material handling for imported Roblox rigs
- Material cleanup for disconnecting Base Color and Alpha inputs
- Automatic Nodes-only armature generation
- Nodes only as the default option in Roblox Animator's Generate Armature dialog
- Automatic matching-part-to-bone constraints after armature generation
- Automatic hiding of generated face bones and weld bones
- Global/Local transform-orientation toggle (`Y`)
- Manual Global/Local orientation controls under Materials
- Automatic installation and updating of the latest Roblox Animator release
- Version information for Roblox Animator and Roblox Animator Utils

The animation shortcuts are intended for use in Pose Mode. The Global/Local transform-orientation shortcut works in Object Mode and Pose Mode.

## Interface

The extensions appear in Blender's N-panel as:

- **Roblox Animator**
- **Roblox Animator Utils**

The Roblox Animator Utils panel includes Materials, transform-orientation controls, compatibility settings, and the Nodes-only armature-generation action.

## Credits

Includes code and functionality from the **Dynamic Parent 2.0.2** extension, updated for Blender 4 compatibility.
