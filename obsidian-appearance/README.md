# Obsidian Appearance Config

My current Obsidian appearance settings, saved so I can sync them to another Mac.

## Current appearance

- **Color scheme:** Dark (`obsidian`)
- **Community CSS theme:** none (default theme)
- **Interface font:** Bear Sans
- **Translucent window:** on
- **Enabled CSS snippet:** `line-spacing`

## How to apply on another Mac

In your target vault's `.obsidian` folder (e.g. `<vault>/.obsidian/`):

1. Copy `appearance.json` into `<vault>/.obsidian/appearance.json`.
2. Copy `snippets/line-spacing.css` into `<vault>/.obsidian/snippets/line-spacing.css`.
3. Make sure the **Bear Sans** font is installed on that Mac (otherwise Obsidian falls back to the default UI font).
4. Restart Obsidian, or in Settings → Appearance toggle the `line-spacing` snippet off/on to reload.

Quick one-liner (replace `<vault>` with the target vault path):

```sh
VAULT="<vault>"
mkdir -p "$VAULT/.obsidian/snippets"
cp appearance.json "$VAULT/.obsidian/appearance.json"
cp snippets/line-spacing.css "$VAULT/.obsidian/snippets/line-spacing.css"
```
