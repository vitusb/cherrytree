# CherryTree

### - Deutsch -

(Die MSI-Pakete sind mit dem [Advanced Installer](https://www.advancedinstaller.com/) von [Caphyon](https://www.caphyon.com/) erstellt worden.)

Dies ist eine gehärtete Version von "cherrytree" für Windows x64-bit Build. Der Patch verhindert, dass "cherrytree" Codeblöcke durch externe Shells ausführt und erzwingt den Wert von "custom_codexec_term" in der "config.cfg" auf "None" zu setzen. Einzelheiten zu den Änderungen finden Sie in der Patch-Datei im Quellbaum. Die Patches sind nicht im Quellcode angewendet, sondern existieren jeweils immer zu dem jeweiligen Release-Stand als Patch-Datei im Quellpfad.

Unbeaufsichtigte synchrone Installation (Exe-Installer Beispiel: gestartete Shell mit administrativen Rechten):<br>
```
start /wait "" "cherrytree_x.x.x.x_win64_disarmed_setup.exe" /LANG=German /VERYSILENT /NORESTART /LOG

start /wait "" "cherrytree_x.x.x.x_win64_disarmed_setup_nolatex.exe" /LANG=German /VERYSILENT /NORESTART /LOG
```
Den öffentlichen OpenPGP-Signaturschlüssel finden sie hier: [vitusb_software_signing_key.zip](https://github.com/vitusb/cherrytree/files/15015491/vitusb_software_signing_key.zip)



### - English -

(The MSI-packages are created by [Advanced Installer](https://www.advancedinstaller.com/) from [Caphyon](https://www.caphyon.com/).)

This is a disarmed version of "cherrytree" for Windows x64 build. The patch prevents "cherrytree" from executing code-blocks by external shells and also forces to set the value of "custom_codexec_term" to "None" in "config.cfg". For details to the changes, look into the patch-file in the source-tree. The patches are not applied in the source code, but always exist at the respective release status as a patch-file in the source-tree.

Unattended synchronous installation (Exe-Installer example: started shell with administrative rights):<br>
```
start /wait "" "cherrytree_x.x.x.x_win64_disarmed_setup.exe" /LANG=English /VERYSILENT /NORESTART /LOG

start /wait "" "cherrytree_x.x.x.x_win64_disarmed_setup_nolatex.exe" /LANG=English /VERYSILENT /NORESTART /LOG
```
You can find the public OpenPGP signature key here: [vitusb_software_signing_key.zip](https://github.com/vitusb/cherrytree/files/15015491/vitusb_software_signing_key.zip)

### - Original Readme follows -

A hierarchical note taking application, featuring rich text and syntax highlighting, storing data in either a single file (xml or sqlite) or multiple files and directories.
The project home page is [giuspen.net/cherrytree](https://www.giuspen.net/cherrytree/).

Written by Giuseppe Penone (aka giuspen) and Evgenii Gurianov (aka txe).

![Cherrytree main window with text](docs/cherrytree-main_window_text.png)

## Features
- Rich text (foreground color, background color, bold, italic, underline, strikethrough, small, h1, h2, h3, h4, h5, h6, subscript, superscript, monospace)
- Syntax highlighting supporting several programming languages
- Images handling: insertion in the text, edit (resize/rotate), save as png file
- Latex math equations rendering
- Embedded files handling: insertion in the text, save to disk
- Multi-level lists handling (bulleted, numbered, to-do and switch between them, multiline with shift+enter)
- Simple tables handling (cells with plain text), cut/copy/paste row, import/export as csv file
- Codeboxes handling: boxes of plain text (optionally with syntax highlighting) into rich text, import/export as text file
- Execution of the code for code nodes and codeboxes; the terminal and the command per syntax highlighting is configurable in the preferences dialog; an embedded terminal is available on linux and mac os
- Alignment of text, images, tables and codeboxes (left/center/right/fill)
- Hyperlinks associated to text and images (links to webpages, links to nodes/nodes + anchors, links to files, links to folders)
- Spell check (using gspell)
- Intra application copy/paste: supported single images, single codeboxes, single tables and a compound selection of rich text, images, codeboxes and tables
- Cross application copy/paste (tested with libreoffice and gmail): supported single images, single codeboxes, single tables and a compound selection of rich text, images, codeboxes and tables
- Copying a list of files from the file manager and pasting in cherrytree will create a list of links to files, images are recognized and inserted in the text
- Print & save as pdf file of a selection / node / node and subnodes / the whole tree
- Export to html of a selection / node / node and subnodes / the whole tree
- Export to plain text of a selection / node / node and subnodes / the whole tree
- Toc generation for a node / node and subnodes / the whole tree, based on headers h1, h2 and h3
- Find a node, find in selected node, find in selected node and subnodes, find in all nodes
- Replace in nodes names, replace in selected node, replace in selected node and subnodes, replace in all nodes
- Iteration of the latest find, iteration of the latest replace, iteration of the latest applied text formatting
- Import from html file, import from folder of html files
- Import from plain text file, import from folder of plain text files
- Import from basket, cherrytree, epim html, gnote, keepnote, keynote, knowit, mempad, notecase, rednotebook, tomboy, treepad lite, tuxcards, zim
- Export to cherrytree file of a selection / node / node and subnodes / the whole tree
- Password protection (using http://www.7-zip.org/) available only for storage as single file – NOTE: while a cherrytree password protected document is opened, an unprotected copy is extracted to a temporary -folder of the filesystem; this copy is removed when you close cherrytree
- Tree nodes drag and drop
- Automatic link to web page if writing the URL
- Automatic link to node if writing node name surrounded by [[node name]]

## Prebuilt binaries
Prebuilt binaries can be found on [github.com/giuspen/cherrytree/releases](https://github.com/giuspen/cherrytree/releases) and [giuspen.net/cherrytree/#downl](https://www.giuspen.net/cherrytree/#downl).

## How to build from source code
In order to build from the source code, please read [BUILDING.md](BUILDING.md).

## Localization
The following languages are supported (If you want to help translating to your language write me):

- Arabic (Abdulrahman Karajeh, up to date)
- Armenian (Seda Stamboltsyan, up to date)
- Bulgarian (Iliya Nikolaev, up to date)
- Chinese Simplified (Wang Yu, up to date)
- Chinese Traditional (Emer Chen, up to date)
- Croatian (Filip Bakula, up to date)
- Czech (Pavel Fric, up to date)
- Dutch (up to date)
- English (default)
- French (Francis Gernet, up to date)
- Finnish (Henri Kaustinen, TO BE UPDATED)
- German (Matthias Hoffmann, up to date)
- Greek (TO BE UPDATED)
- Hindi India (TO BE UPDATED)
- Hungarian (Stiener Norbert, TO BE UPDATED)
- Italian (Vincenzo Reale, up to date)
- Japanese (Piyo, up to date)
- Kazakh (Viktor Polyanskiy, up to date)
- Kazakh (Latin) (Viktor Polyanskiy, up to date)
- Korean (Sean Lee, up to date)
- Lithuanian (up to date)
- Persian (Majid Abri, up to date)
- Polish (Mariusz Gasperaniec, up to date)
- Portuguese (Rui Santos, up to date)
- Portuguese Brazil (Raysa Dutra, up to date)
- Romanian (Tudor Sprinceana, up to date)
- Russian (Viktor Polyanskiy, up to date)
- Slovenian (Erik Lovrič, up to date)
- Spanish (up to date)
- Swedish (Åke Engelbrektson, up to date)
- Turkish (Ferhat Aydin, up to date)
- Ukrainian (Giuseppe Penone, up to date)

## Used libraries
https://www.gtkmm.org/en/documentation.shtml
https://developer-old.gnome.org/gtkmm-tutorial/3.24/
https://developer-old.gnome.org/gtkmm/3.24/
https://developer-old.gnome.org/gtkmm/3.24/hierarchy.html

https://developer-old.gnome.org/gtksourceviewmm/stable/

https://developer-old.gnome.org/libxml++-tutorial/stable/
https://developer-old.gnome.org/libxml++/stable/

https://wiki.gnome.org/Projects/gspell
https://developer-old.gnome.org/gspell/stable/
