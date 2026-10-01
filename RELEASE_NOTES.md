# EchelDraw 0.1.9

A fix for texts created by agents. Drawings, settings and personal libraries
from 0.1.8 remain compatible; the plugin ID remains `eddraw`.

- Texts that an agent (MCP) creates or edits right after Obsidian opens no
  longer lose their last letter. The plugin now loads the text's font before
  measuring it, so the text box has the right width in every font.

Install or update with BRAT using `EchelOneZero/echeldraw-obsidian`, or download
`echeldraw-0.1.9.zip` and copy its three files into the existing plugin folder.
When updating manually, preserve `data.json`, `personal-library.json` and
recovery files.

Requires Obsidian desktop 1.13.7 or later.
