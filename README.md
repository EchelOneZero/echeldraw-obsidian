# EchelDraw for Obsidian

Draw flowcharts, mind maps and freehand diagrams directly in your Obsidian vault.
EchelDraw uses the Excalidraw editor with additional diagram tools, note cards,
drawing previews and a personal library. Drawings are ordinary `.excalidraw`
files stored in your vault.

**Desktop only. Requires Obsidian 1.13.7 or later.**

EchelDraw is the new name of EdDraw starting with version 0.1.2. It keeps the
same plugin ID (`eddraw`) and installation folder so existing vaults retain their
settings, personal libraries and drawings. Existing project folders keep their
paths; new installations default to `EchelDraw` for newly created projects.

## Install with BRAT

Repeat these steps in each vault where you want EchelDraw:

1. In **Settings → Community plugins → Browse**, install and enable **BRAT**.
2. Open BRAT's settings and choose **Add beta plugin**, or run **BRAT: Add a
   beta plugin for testing** from the command palette.
3. Enter `https://github.com/EchelOneZero/echeldraw-obsidian` and choose the latest
   version.
4. Enable **EchelDraw** in Community plugins if it is not enabled automatically.

BRAT installs and updates the package from this repository's GitHub Releases.
EchelDraw is not currently listed in Obsidian's official Community Plugins catalog.
Disable another Excalidraw plugin in this vault before enabling EchelDraw because
both plugins handle the `.excalidraw` extension.

## Install manually

1. Download `echeldraw-0.1.2.zip` from [Releases](https://github.com/EchelOneZero/echeldraw-obsidian/releases/latest).
2. Close Obsidian and extract the ZIP directly into
   `<vault>/.obsidian/plugins/eddraw/`.
3. `main.js`, `manifest.json` and `styles.css` must be directly inside `eddraw/`.
4. Reopen Obsidian and enable **EchelDraw** in Community plugins.

The release assets also include these three files individually for BRAT. The
GitHub **Source code** archives contain repository documentation and are not the
installable plugin.

## Use EchelDraw

- Run **EchelDraw: Gerenciar desenhos** to manage drawings in your vault.
- Right-click a folder and choose **Novo desenho EchelDraw nesta pasta** to create
  a drawing there.
- Use **EchelDraw: Criar desenho e inserir link na nota** to link a new drawing from
  a note.
- Insert Markdown notes as cards in a drawing, or insert a PNG drawing preview
  in a note with a link to the editable file.
- Configure the theme, new-drawing background, default arrowhead and personal
  library under **Settings → EchelDraw**. The interface is currently in Portuguese.

## Storage and updates

Drawings stay in the vault. Preferences are stored in the plugin's `data.json`;
personal library items are stored in `personal-library.json`, with a recovery
copy in `personal-library.backup.json`. Each vault has its own settings and
library. Installing on another computer does not copy your drawings or settings;
transfer or sync your vault separately if you want the same content.

Keep these data files when updating manually. BRAT updates the installed bundle
files. Editor code, fonts and the brand icon catalog are embedded in the package,
so no additional runtime or asset folders are required. The editor initializes
when the first drawing is opened; brand icons are indexed on their first search.
The package does not include preset library collections.

## Network use and privacy

Editing drawings, fonts and brand icon search work locally. The plugin does not
include telemetry and does not require an account or a running web server.

- **Favicon de site** contacts the website you enter to retrieve its icon only
  when you use that feature.
- **Itens pessoais da versão web → Copiar itens** contacts the optional local
  Operation Center at `http://localhost:4500/draw/api/libraries/personal` only
  when requested. This is a one-time copy, and drawings remain independent of
  the web application.
- BRAT uses GitHub to install and check for updates.

## License and credits

EchelDraw is released under the [MIT license](LICENSE). It is an independent plugin,
not an official Obsidian product. It is built with [Excalidraw](https://github.com/excalidraw/excalidraw),
[React](https://github.com/facebook/react), [Lucide](https://github.com/lucide-icons/lucide),
and [Simple Icons](https://github.com/simple-icons/simple-icons).

Dependencies and fonts retain their respective licenses. Full notices are in
[THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) and in the readable header of
`main.js`. Brand logos and trademarks belong to their respective owners.

This public repository contains release metadata, documentation and downloadable
bundles. The development source repository is currently private; bundled code is
distributed under the stated licenses.
