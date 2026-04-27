# MindLite

MindLite is a self-contained browser-based mind mapping app distributed as a single HTML file.

The project currently ships as [`MindLite.html`](./MindLite.html) with no build step, no package manager, and no external runtime dependencies. Open the file in a modern desktop browser and start working.

Current release: `v0.3.0`

## Core Features

- Creates a central topic and child nodes on an infinite canvas
- Supports moving, resizing, folding, and reattaching branches
- Supports text styling for nodes and hyperlinks
- Saves editable mind maps as standalone HTML files
- Saves encrypted working copies and encrypted shared HTML copies with a password
- Exports read-only shareable HTML, landscape PDF output, and PDF ZIP packages with attachments
- Lets you pin mind maps by their central nodes and jump back to them from the toolbar
- Supports pasting screenshots or images directly onto the canvas
- Supports attaching PDF, Word, PowerPoint, Markdown, Quarto, and RTF documents to nodes
- Adds hyperlinks with custom names that can float on the canvas, attach into a node file list, or append under a node
- Renders inline LaTeX with the bundled KaTeX runtime

## Run Locally

1. Open `MindLite.html` in a browser.
2. Click the root button to create the central node.
3. Use the `+` control on a node to add child nodes.
4. Drag empty canvas space to pan.
5. Use the zoom controls, or hold `Ctrl` and scroll, to zoom.
6. Click the hyperlink toolbar button to add a URL with a custom name.

## Editing and Sharing

- `Save` writes a standalone working copy with the current mind map state embedded in the file.
- `Save with password` writes a standalone working copy whose mind map payload is encrypted with the password.
- The reset icon restores the current editable file back to the blank app state.
- `Share As -> HTML` exports a read-only HTML version for sharing.
- `Share As -> HTML with password` exports a read-only HTML version with the mind map payload encrypted.
- `Share As -> PDF` opens a print-ready landscape export flow.
- `Share As -> ZIP` exports a PDF package with `mindmap.pdf`, attached files, and attached/appended URL records.
- Press `Del` to remove a selected node or link.
- Paste an image or screenshot onto the canvas to create an image node.
- Drag a detached node onto another node to attach it as a child.
- Drag supported files onto a node, or use the attachment button, to store file attachments inside the exported document.
- In shared HTML and editor mode, `Ctrl+click` or `Cmd+click` opens hyperlinks and attached URL rows in a new tab or window; plain click does not open them.
- Drag a hyperlink onto a node to choose whether it should attach into the file list or append under the node.


## Notes

- MindLite is currently a single-file app, which means `MindLite.html` is both the source file you edit and the app file you run or share.
- Exported editable and share copies are ignored by `.gitignore`, which means generated files like `mindlite-save-...html` and `mindlite-share-...html` will not be tracked by Git if you save them in this folder.
- The `working in progress` mark appears whenever an editable file contains mind map state, and the reset icon restores that file to the same blank state as the original app.

## Licence

MIT
