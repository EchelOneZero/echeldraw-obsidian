# EchelDraw 0.1.10

Faster dragging in large drawings. Drawings, settings and personal libraries
from 0.1.9 remain compatible; the plugin ID remains `eddraw`.

- Dragging many selected elements no longer rescans the whole drawing on every
  frame. In a test drawing with 2,500 elements, dragging 80 of them used about
  half the CPU and no longer froze for a frame.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.10.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
