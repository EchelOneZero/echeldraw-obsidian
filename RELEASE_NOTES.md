# EchelDraw 0.1.6

New defaults for snapping and for new texts. Drawings, settings and personal
libraries from 0.1.5 remain compatible; the plugin ID remains `eddraw`.

Snap to objects:

- Drawings now open with "snap to objects" turned on.
- If you turn it off in a drawing, that drawing remembers it and reopens with
  it off. Drawings that keep the default are not changed on disk.

New texts:

- A text created with the text tool now starts as a text box: background,
  border and rounded corners, 5 px of padding, centered.
- While the border keeps its default, choosing a background color also paints
  the border with it; once you pick a border color yourself, it stays.
- Creating a text is still a single undo step, and undoing it also removes the
  box. Existing texts, labels inside shapes and on arrows, flow and mind map
  texts and texts created by agents keep their style.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.6.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
