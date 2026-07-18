# Staticaliza's Blender Animation Tools for Roblox

Staticaliza's Blender Animation Tools is a Blender extension package for importing, preparing, and animating Roblox rigs. It installs and works alongside [Cautioned's Roblox Animator](https://github.com/Cautioned/Blender-Animations-Plugin), then adds a streamlined workflow through the **Roblox Animator Utils** N-panel.

## Compatibility

- Roblox Animator Utils 1.6.1
- Blender 4.2 through Blender 5.2
- Roblox Animator 2.6.3 and compatible newer releases
- Windows, macOS, and Linux where Blender extensions and Roblox Animator are supported

Most animation tools are intended for **Pose Mode**.

## Installation

1. Download `Staticaliza's Blender Animation Tools.zip`.
2. Open Blender and select **Edit > Preferences > Get Extensions**.
3. Open the extensions menu and choose **Install from Disk**.
4. Select the downloaded ZIP.
5. Enable **Staticaliza's Blender Animation Tools** if Blender does not enable it automatically.

The lightweight setup extension downloads, installs, and enables the latest versions of:

- **Roblox Animator**: Cautioned's Blender Animations Plugin
- **Roblox Animator Utils**: Staticaliza's animation utilities

The two interfaces appear in the 3D Viewport N-panel as:

- **Roblox Animator**
- **Roblox Animator Utils**

Use **Install Latest Extension** in Roblox Animator Utils to update both extensions later.

## Recommended Roblox Plugins

The **Install Roblox Plugins** button opens both recommended Roblox Creator Store pages:

- [Roblox Blender Animation Tools](https://create.roblox.com/store/asset/118148792788940)
- [Companion Roblox animation plugin](https://create.roblox.com/store/asset/16708835782)

These plugins export Roblox rigs in the format consumed by Roblox Animator's Blender importer.

## Features

### Scene Setup

- Loads the bundled animation template with its saved UI layout and viewport shading.
- Includes a packed Baseplate texture that remains available on other devices and through undo operations.
- Uses one bundled template compatible with the supported Blender range.
- Warns before replacing the current scene and discarding unsaved changes.

### Onion Tools

- Toggle Onion Skin previews for nearby animation poses.
- Preview meshes, bones, or both in Advanced Mode.
- Optional opacity, raycast, and hidden-object controls.
- Create Smart pins at the connected object's lower surface.
- Bone End and Bone Center pin-position modes.
- Update, hide, show, remove, or clear pins.
- Pivot selected bones directly to pins.
- Pivot and stretch from a fixed bone start until the pin is reached.
- Correct handling for rotated parts and numbered helper-bone chains.

### Dynamic Tools

- Dynamic Parent Start and End markers.
- Dynamic Unparent Start and End markers.
- World-transform preservation when relationships change.
- Dynamic Parent and Dynamic Unparent can be combined on the same animation.
- Sparse runtime transition keys instead of inserting keys on every frame.
- Automatic dense evaluation when exporting through Roblox Animator.
- Clear controls in standard mode and optional manual Bake controls in Advanced Mode.

### Surface Contact

- Locks the selected bone's connected object hull against the nearest floor, wall, slope, or custom mesh.
- Includes rigidly welded, layered, and weighted meshes connected to the same numbered bone family.
- Uses a direct world-space bone lock instead of stacking another IK solver, preventing torso movement from forcing the contacted object through a surface.
- Works alongside an existing IK setup and hands control back to its original target when the contact is released.
- Keeps contacts isolated by segment, so a later contact cannot pull a limb away from the current one while seeking or playing.
- Creates an off key on the frame before contact and an on key at contact start, preventing the lock from affecting earlier animation.
- Uses stepped influence states with Automatic keyframe handles rather than Automatic Clamped handles.
- Releases without a visible pose jump.
- Follows animated contact surfaces and preserves contacts after saving and reopening the project.
- Displays active contacts with a hot-pink surface guide in the 3D Viewport.
- Includes contact-controlled bones in Roblox Animator's dense export evaluation.

### Transform Tools

- Switch between Global and Local transform orientation.
- Switch between Blender's normal Bone pivot and an Object-based pivot.
- Object pivot mode uses the first connected rig object's center and orientation.
- Remembers the last transform tool used in Pose Mode.

### Camera Tools

- Create or remove a camera attached to the selected bone.
- Keyframe a bone-attached or standalone camera from the current viewport.
- Cameras remain attached to their bones without offset jumps.
- Orientation presets for `+X`, `-X`, `+Y`, `-Y`, `+Z`, and `-Z`.
- Default `-Z` camera orientation.
- Cinematic preset at 35 degrees.
- Classic preset at 70 degrees.
- Custom field-of-view mode.
- Optional hiding of the camera's attached object in the viewport and render.

### Materials And Textures

- Smart Material Import detects Roblox rig collections automatically.
- If a Principled BSDF has both Base Color and Normal connected, only Base Color is disconnected.
- Optional viewport material standardization to `#E7E7E7`, metallic `0`, and roughness `0.5`.
- Optional clothing-layer clipping prevention, disabled by default.
- **Clear** disconnects Base Color and Alpha while preserving the bundled Baseplate material.
- Imported rig materials and images are isolated per rig.
- Textures are reloaded fresh, uniquely namespaced, and packed into the Blender file.
- Later imports cannot replace the texture already assigned to an earlier rig.

> [!IMPORTANT]
> Export each Roblox rig into its own folder. If multiple exports overwrite the same PNG files before Blender imports them, the original pixels are already lost and cannot be recovered by the extension. Rigs that were previously assigned the wrong image must be re-exported and re-imported.

### Roblox Rig Compatibility

- Detects multiple valid `RIG: Name` collections in the same scene.
- Supports matching `Parts`, `__Name_Armature`, and `__NameMeta` data.
- Automatically generates Local Y-axis-aligned armatures when Advanced Mode is off.
- Leaves armature generation manual when Advanced Mode is on.
- Automatically applies matching-part-to-bone constraints.
- Avoids duplicate constraints and weak duplicate weld behavior.
- Hides weld bones, face bones, numbered helper bones, and auxiliary bone collections in standard mode.
- Hides matching `__NameMeta` empty objects from the viewport and selection.
- Hides bone axes, labels, relationship lines, and advanced Roblox Animator panels in standard mode.
- When bone names are enabled, selecting bones temporarily shows only the active bone's label using Blender's native label styling; deselecting all bones restores every label.
- Restores advanced panels and auxiliary controls when Advanced Mode is enabled.
- Uses Automatic keyframe handles rather than Automatic Clamped handles.
- Expands a newly created Dope Sheet channel when its first keyframe is inserted.

## Shortcuts

| Shortcut | Action | Primary Mode |
| --- | --- | --- |
| `F` | Toggle Onion Skin | Pose Mode |
| `Shift + F` | Create or manage Onion Pins | Pose Mode |
| `Alt + F` | Dynamic Parent and Dynamic Unparent menu | Pose or Object Mode |
| `Y` | Switch Global/Local orientation | Pose or Object Mode |
| `Shift + Y` | Switch Bone/Object pivot | Pose Mode |
| `Ctrl + Alt + NumPad 0` | Keyframe the selected camera bone or standalone camera | 3D View/Pose Mode |

The Onion and Dynamic shortcuts are also registered in the Dope Sheet and Graph Editor where applicable.

## Advanced Mode

Advanced Mode is disabled by default. Enabling it exposes detailed controls such as:

- Onion Skin opacity, mesh, bone, raycast, and hidden-object options
- Smart Material Import settings
- Viewport material standardization
- Clothing clipping prevention
- Dynamic Parent and Dynamic Unparent Bake buttons
- Roblox Animator armature-generation and rigging controls
- Weld, face, helper, axis, label, and relationship-line visibility
- Additional Roblox Animator account, validation, import, mapping, and export options
- Surface-detection filtering

## Release Files

| File | Purpose | When To Upload |
| --- | --- | --- |
| `Staticaliza's Blender Animation Tools.zip` | Lightweight setup extension downloaded by users | Only when setup/downloader code changes |
| `src/staticaliza_blender_animation_tools.zip` | Roblox Animator Utils source payload fetched by setup | Whenever Utils code, templates, or version changes |

Roblox Animator itself is downloaded directly from Cautioned's latest GitHub release and is not bundled in either ZIP.

## Building Release ZIPs

From the repository folder on Windows:

- Double-click `Build Source ZIP.cmd` after changing Roblox Animator Utils.
- Double-click `Build Setup ZIP.cmd` after changing the setup/downloader.
- Run `Build Staticaliza Global Setup.ps1` to rebuild both.

Generated files are written to the release paths shown above. Temporary download and packaging files are not included.

## Credits

- [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin) for Roblox Animator importing, rigging, animation, and export functionality.
- **Dynamic Parent 2.0.2** by Roman Volodin for the original Dynamic Parent implementation, updated here for Blender 4.2 through 5.2 and integrated with Roblox animation export.

## License

Roblox Animator Utils is distributed under the GNU General Public License v2.0 or later. See the source headers and extension manifest for details.
