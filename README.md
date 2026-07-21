# Staticaliza's Blender Animation Tools for Roblox

<p align="center">
  <img src="docs/logo.png" alt="Staticaliza's Blender Animation Tools">
</p>

Roblox Animator Utils supports **Blender 4.2 through Blender 5.2**. Most animation tools are intended for Pose Mode.

Staticaliza's Blender Animation Tools installs [Cautioned's Roblox Animator](https://github.com/Cautioned/Blender-Animations-Plugin) and adds the **Roblox Animator Utils** workflow for importing, preparing, animating, and exporting Roblox rigs.

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

- **Animation Tools**: Dynamic Parent, Dynamic Unparent, Surface Contact, and single- or multi-bone cameras in the `Ctrl + F` menu and N-panel.
- **Active Armatures**: Edit one or several rigs in Pose Mode while inactive rigs keep their visible meshes but hide bones, colors, names, pins, contacts, and onion previews.
- **Rig Cleanup**: Delete an imported rig from Active Armatures with one undoable action, including its exclusive collection, parts, helpers, animation data, materials, and textures while preserving shared assets.
- **Multi-Rig Feedback**: Same-named bones stay tied to the correct rig. Enabled rigs receive yellow rig labels, the active rig is emphasized, and inactive rig labels appear on hover.
- **Onion Tools**: Per-rig mesh and bone previews, selectable yellow Onion Pins and pink Contact targets, free center or axis dragging, connected-object placement, and snap rings.
- **Pin Transforms**: Select pins alone or Shift-select them with bones, use `G`, `R`, and `S`, and switch between Bone and Object pivots without showing Blender's bone gizmo for pin-only selection.
- **Surface Contact**: Create contacts for one or several selected endpoints at once, with no-stretch simulation, exact dot-to-dot locking, one-sided collision, surface-gliding targets, moving-surface tracking, and reuse of genuine existing IK chains.
- **State Feedback**: Parent, Unparent, and Surface Contact states merge their bone colors and display ordered status labels. Ordinary bone channels stay alphabetical above consistently ordered special channels. Onion Pin remains a yellow marker-only state, and overlapping Pin/Contact markers use a blended color.
- **Viewport Workflow**: Free-view position, shading, lighting, overlays, clipping, lens, and gizmo settings stay synchronized across animation workspaces; Animate and Graph also share N-sidebar visibility, active tab, and scroll position.
- **Camera Tools**: Attach bone-tip cameras to one or several selected bones, with adjustable FOV presets, local-axis orientation, attached-object hiding, and keyframing that enters camera view.
- **Rig Setup**: New rigs enter Pose Mode automatically, Action channels expand to the bone level, and generated rigs receive Local Y-axis armatures, matching-part constraints, duplicate-weld prevention, and helper-bone hiding.
- **Materials**: Smart material import, safe Base Color and Alpha clearing, per-rig texture isolation, viewport standardization, and optional clothing-clipping prevention.
- **Export**: Dynamic relationships and contacts are densely evaluated through Roblox Animator, while untouched bones with no authored keys are omitted for partial-body animation layering.
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

## Credits

- [Cautioned/Blender-Animations-Plugin](https://github.com/Cautioned/Blender-Animations-Plugin)
- **Dynamic Parent 2.0.2** by Roman Volodin, updated for Blender 4.2 through 5.2 and Roblox animation export.

## License

Roblox Animator Utils is distributed under the GNU General Public License v2.0 or later.
