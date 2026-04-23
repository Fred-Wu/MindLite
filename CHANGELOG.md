# Changelog

All notable changes to MindLite are documented in this file.

## [0.2.0] - 2026-04-23

### Added

- Added hyperlink creation from the toolbar with URL and custom-name input.
- Added hyperlink placement modes so links can remain free on the canvas, attach into a node file list, or append beneath a node.
- Added hyperlink text styling support for font family, size, bold, and italic.
- Added duplicate-name protection across hyperlinks and references.
- Added stricter hyperlink URL validation with direct user feedback before saving.
- Added "READ ONLY" marker in a shared HTML output.

### Changed

- Changed new text nodes to start middle-centered and narrower than before.
- Changed the help and project documentation to describe the current hyperlink workflow and current app behavior.
- Reduced the attachment button circle and child-node `+` button circle slightly.

### Fixed

- Fixed node dragging so fast pointer movement keeps a locked grabbing cursor and no longer drops visually back to the canvas mid-drag.
- Fixed node edge dragging so starting a drag from the border more reliably moves the node instead of panning the canvas.

## [0.1.1] - 2026-04-22

### Added

- Added text style toolbar controls for size, bold, and italic formatting.
- Expanded the node font picker with a broader set of common UI-oriented font families.

### Changed

- Set Optima as the default font for node text input without changing the rest of the app UI text.
- Changed node text to use normal weight and style by default instead of the earlier heavier default.
- Removed node fill color and reduced text-node interior spacing to the current tighter layout, with only a small left/right inset remaining.
- Widened the font picker slightly so the default Optima label is fully visible in the closed control.

### Fixed

- Fixed new text nodes so they start at their settled height instead of shrinking on first blur.
- Fixed middle vertical alignment so typed text is centered correctly in newly created nodes.
- Fixed the text-style toolbar so it keeps showing the current node font state when selection is cleared instead of falling back to the default font display.

## [0.1.0] - 2026-04-22

### Added

- Initial tracked release of the single-file MindLite app.
- Added a toolbar reset action that restores the current editable file back to the blank app state.
