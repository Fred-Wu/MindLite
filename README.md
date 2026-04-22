# MindLite

MindLite is a self-contained browser-based mind mapping app distributed as a single HTML file.

The project currently ships as [`MindLite.html`](./MindLite.html) with no build step, no package manager, and no external runtime dependencies. Open the file in a modern desktop browser and start working.

## What It Does

- Creates a central topic and child nodes on an infinite canvas
- Supports moving, resizing, folding, and reattaching branches
- Saves editable mind maps as standalone HTML files
- Exports read-only shareable HTML and landscape PDF output
- Lets you pin hidden references and jump back to them from the toolbar
- Supports pasting screenshots or images directly onto the canvas
- Supports attaching PDF and Office documents to nodes
- Renders inline LaTeX with the bundled KaTeX runtime

## Project Layout

```text
MindLite/
├── CHANGELOG.md
├── MindLite.html
├── README.md
└── .gitignore
```

## Run Locally

1. Open `MindLite.html` in a browser.
2. Click the root button to create the central node.
3. Use the `+` control on a node to add child nodes.
4. Drag empty canvas space to pan.
5. Use the zoom controls, or hold `Ctrl` and scroll, to zoom.

## Editing and Sharing

- `Save` writes a standalone working copy with the current mind map state embedded in the file.
- The reset icon restores the current editable file back to the blank app state.
- `Share As -> HTML` exports a read-only HTML version for sharing.
- `Share As -> PDF` opens a print-ready landscape export flow.
- Press `Del` to remove a selected node or link.
- Paste an image or screenshot onto the canvas to create an image node.
- Drag a detached node onto another node to attach it as a child.
- Drag supported files onto a node, or use the attachment button, to store file attachments inside the exported document.


## Notes

- MindLite is currently a single-file app, which means `MindLite.html` is both the source file you edit and the app file you run or share.
- Exported editable and share copies are ignored by `.gitignore`, which means generated files like `mindlite-save-...html` and `mindlite-share-...html` will not be tracked by Git if you save them in this folder.
- The `working in progress` mark appears whenever an editable file contains mind map state, and the reset icon restores that file to the same blank state as the original app.

## Licence

MIT
