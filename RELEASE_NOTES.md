# EchelDraw 0.1.8

List markers of one size, and text color defaults that stick. Drawings,
settings and personal libraries from 0.1.7 remain compatible; the plugin ID
remains `eddraw`.

List markers:

- Every list marker now has the same size, so the text of a list stays in one
  column. Before, a checked task (☑) could show as a large emoji and an open
  one (☐) as a small symbol.
- An open task is an empty square with a red border, a done task is the same
  square in green with a white check, and a cancelled task is gray with an X.
  Bullets, milestones (◇/◆), steps and quotes use the text color.
- The text keeps the same characters, so existing drawings, editing and
  agents are unchanged; exports and previews show the new markers too.

Text color:

- New texts start black. If you change a text's color in a drawing, the next
  texts in that drawing keep that color, including texts created by double
  click on the canvas or inside a shape, and it is saved with the drawing.
- Changing the color of a shape no longer changes the color of the next text.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.8.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
