# State Manager
**State Manager (Continued) is a maintained fork of the original State Manager extension for AUTOMATIC1111 WebUIs.**

It lets you save and restore your full UI setup for `txt2img` and `img2img`, so you can jump back to a working configuration without rebuilding everything by hand.

If you've ever lost track of which model, sampler, or script settings you were using between runs, that's the problem this solves. Save your setup, browse your history, keep reusable configs, and bring back either the whole thing or just the parts you need.

<img width="270" alt="preview-modal" src="https://github.com/user-attachments/assets/eabca34a-0229-46ca-b544-ee9efe88d3b9" /> <img width="270" alt="preview-small" src="https://github.com/user-attachments/assets/e37a78f9-8517-4097-834f-731049236871" /> <img width="270" alt="preview-quick" src="https://github.com/user-attachments/assets/eff429c2-ec3e-4590-ba2e-6eb6d23cff45" />

## Core Features

- **Save and restore your full setup** - captures everything in your `txt2img`/`img2img` tab so you can get back to a known-good state in one click.
- **History + Configs with flexible apply** - generated states are kept in `History`, reusable presets live in `Configs`. Apply a full config or just the parts you want.
- **Modal, small view, and quick menu** - modal gives you a full workspace, small view keeps things compact alongside your tabs, and the quick menu shows up to 10 configs as tiles for fast one-click access. Modal can be opened from either view.
- **Collapsible small view** - collapse or expand the small-view section with a chevron toggle. State persists between sessions.
- **Draft-based config editing** - changes aren't saved automatically. `Save Changes` stays disabled until you edit something, and you'll get a prompt if you try to navigate away with unsaved changes.
- **Config duplication** - rename an existing config and save it as a new copy.
- **Config card gear menu** - swap a config's preview image through the gear icon on its card.
- **Manual config ordering** - reorder your configs in the Configs tab with arrow controls. The order carries over to the quick menu.
- **Filtering and sorting** - search by key fields, sort and group entries, and optionally remember your last-used filters between sessions.
- **Startup Config** - pick a config to auto-apply when WebUI launches, or set it to `None` to start fresh.
- **Settings tab** - a dedicated tab for all preferences: entry counts, pagination, timestamps, date format, default sort, default tab, search bar visibility, apply safety checks, and more. All persisted in IndexedDB.
- **Management** - rename, save, copy, delete, and unsave configs. Multi-select with modifier keys for batch actions.

## Usage

State Manager adds a panel to your `txt2img` and `img2img` tabs where you can browse your saved `History` entries and reusable `Configs`.

**Saving configs** - click `Save Current UI as Config` to capture your current settings as a named config. To duplicate an existing config, rename it and use `Save as Config` to create a copy.

**Applying configs** - select an entry and click `Apply Config` to restore the full setup, or open the inspector and check only the parts you want to apply. Double-clicking an entry applies it immediately.

**Quick access** - the quick menu shows up to 10 of your saved configs as tiles. Click one to select it, then hit `Apply Config` at the top. If you need more room, expand to the small view or open the modal for a full workspace.

**Config ordering** - in the Configs tab, enter `Reorder` mode to rearrange your configs with the arrow controls. The order carries over to the quick menu.

**Customizing behavior** - open the `Settings` tab to adjust things like which tab opens by default, whether filters are remembered, timestamp display, pagination, and more. Set a `Startup Config` here if you want WebUI to launch with a specific setup already applied.

**Editing configs** - changes in the inspector are tracked as drafts and aren't saved until you hit `Save Changes`. If you try to navigate away with unsaved edits, you'll get a prompt. You can also swap a config's preview image through the gear icon on its card.

## Installation

1. Open AUTOMATIC1111 WebUI.
2. Go to `Extensions > Install from URL`.
3. Paste:

```text
https://github.com/dane-9/sd-webui-state-manager-continued
```

4. Click `Install`.
5. Restart WebUI.