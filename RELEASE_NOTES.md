# EchelDraw 0.1.7

Style defaults per element type. Drawings, settings and personal libraries
from 0.1.6 remain compatible; the plugin ID remains `eddraw`.

Defaults in each drawing:

- The last style change you make to an element type in a drawing (rectangle,
  diamond, ellipse, arrow, line, free drawing or text) becomes that type's
  default in the drawing. Picking the tool again starts with that style.
- A type without its own default starts with the style the drawing opened
  with, so a color chosen for rectangles does not carry over to ellipses.
- For texts, the default also includes the text box chosen last.
- The defaults are saved in the drawing file and survive closing, reopening
  and agent edits. Drawings where you change nothing are not changed on disk.

App defaults:

- Right-click a selection of one element type and choose "Definir como padrão
  do app" to use its style in every drawing that has no default of its own for
  that type. It is saved in the plugin settings.
- Order of precedence: the drawing's default, then the app's, then the
  original style.

Applying a default does not add an undo step. Undoing a style change does not
undo the default it recorded; change the style again to replace it.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.7.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
