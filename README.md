# Staticaliza's Blender Animation Tools for Roblox/Blender

This Blender extension, which currently only supports Blender 4.3.0, adds additional Roblox animation tools and works alongside [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin), which supports importing and animating Roblox rigs in Blender.

It is recommended to install the [Roblox Blender Animation Tools plugin](https://create.roblox.com/store/asset/118148792788940), which allows avatar rigs to be imported into Blender using Cautioned's animation plugin.

## Automatic Setup

Install `Staticaliza's Blender Animation Tools.zip` through Blender's **Install from Disk** option.

The setup extension automatically downloads, installs, and enables the latest versions of:

- **Roblox Animator**: Cautioned's Blender Animations Plugin
- **Roblox Animator Utils**: Staticaliza's Blender Animation Tools

The setup extension also displays the installed version of each extension. Downloaded temporary files are automatically removed after installation.

## Features

- Onion Skins (`F`)
- Onion Pins (`Shift + F`)
- Unparent with start and end keyframes (`Alt + F`)
- Dynamic Parent with start and end keyframes (`Shift + Alt + F`)
- Automatic material handling for imported rigs
- Smart Material Import
- Automatic Nodes-only armature generation
- Automatic matching-part-to-bone constraints
- Automatic hiding of generated face bones and weld bones
- Automatic installation and updating of Cautioned's latest Roblox Animator release

The animation shortcuts are intended for use in Pose Mode.

## Interface

The extensions appear in Blender's N-panel as:

- **Roblox Animator**
- **Roblox Animator Utils**

## Credits

Includes code and functionality from the **Dynamic Parent 2.0.2** extension, updated for Blender 4 compatibility.
