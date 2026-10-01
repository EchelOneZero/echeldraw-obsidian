# EchelDraw 0.1.4

Grouped shapes now work as flow blocks. Drawings, settings and personal
libraries from 0.1.3 remain compatible; the plugin ID remains `eddraw`.

Flow with groups:

- Selecting a group, such as a card with a title, shows the flow controls:
  the `+` handles around the whole group, "Trocar tipo" (change type) and
  "Duplicar ramo" (duplicate branch). Arrows attach to the group's largest
  shape.
- In the next-step picker, "Mesmo tipo" (same type) repeats the whole group as
  a template: the shape, its titles and their text boxes, in a new group,
  connected to the original. One undo removes the copy. Other types still
  create only the shape.
- "Trocar tipo" keeps the shape in its group, and "Duplicar ramo" also copies
  the titles and notes grouped with the duplicated shapes.
- The keyboard shortcuts that add the next step also work with a group
  selected.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.4.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
