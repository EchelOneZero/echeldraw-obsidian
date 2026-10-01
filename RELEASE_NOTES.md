# EchelDraw 0.1.3

A reliability update for undo, saving and text boxes. Drawings, settings and
personal libraries from 0.1.2 remain compatible; the plugin ID remains `eddraw`.

Undo and styles:

- Dragging a slider or picking a color in the text box and frame panels now
  creates a single undo step for the whole gesture, instead of one per step.
- The first style applied to a shape or frame can be undone.
- Undo no longer brings back a style that was already undone after a slider
  was released on its original value.
- The text box panel no longer reopens or closes its groups while you edit.
- Formatting the label of an arrow keeps the arrow connected to its shapes.

Connections and text boxes:

- Deleting an arrow and undoing brings back its label.
- Double-clicking an arrow with a positioned label edits that label instead of
  creating a second one.
- Text boxes follow their text while you drag, resize or type, and one undo
  restores both.
- The label size and position fields apply when you confirm the value, not on
  every key.

Saving:

- Edits are saved at most a few seconds after you stop, even during long
  continuous edits, and pending edits are saved when Obsidian quits.
- Large drawings save faster while you move elements.
- Recovery data for unsaved edits has a size limit, so it no longer competes
  with other plugins for local storage.
- Note previews hide collapsed mind map branches.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.3.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
