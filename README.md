# State Manager
**State Manager (Continued) is a maintained fork of the original State Manager extension for AUTOMATIC1111 WebUIs.**

It lets you save and restore your full UI setup for `txt2img` and `img2img`, so you can jump back to a working configuration without rebuilding everything by hand.

If you've ever lost track of which model, sampler, or script settings you were using between runs — that's the problem this solves. Save your setup, browse your history, keep reusable configs, and bring back either the whole thing or just the parts you need.

<img width="270" alt="preview-modal" src="https://github.com/user-attachments/assets/eabca34a-0229-46ca-b544-ee9efe88d3b9" /> <img width="270" alt="preview-small" src="https://github.com/user-attachments/assets/e37a78f9-8517-4097-834f-731049236871" /> <img width="270" alt="preview-quick" src="https://github.com/user-attachments/assets/eff429c2-ec3e-4590-ba2e-6eb6d23cff45" />

## Core Features

- **Save and restore your full setup**  
  Captures everything in your `txt2img`/`img2img` tab so you can get back to a known-good state in one click.
- **History + Configs with flexible apply**  
  Your generated states are kept in `History`, and you can save reusable presets to `Configs`. Apply a full config or just pick the parts you want.
- **Manual config ordering**  
  Adjust the order your saved configs show up in, the quick view will display the first 10 configs.
- **Filtering and sorting**  
  Search by key fields and change how things are sorted or grouped to find what you're looking for faster.
- **Modal, small view, and quick menu**  
  Modal view gives you a full workspace, small view keeps things compact alongside your tabs, and the quick menu provides fast one-click access to your configs.
- **Startup Config**  
  Pick a config to auto-apply when WebUI launches, or set it to `None` to start fresh.
- **Settings and management**  
  Tweak things like `Startup Config`, `Remember Last-Used Filters`, `Default Open Tab`, sort/display options, and safety checks. Manage entries with rename, save, copy, delete, and batch actions.

## Usage

State Manager adds a panel where you can browse your `History` and `Configs`, see what's saved in each one, and apply the full setup or just specific parts. You can save your current UI state as a named config, reorder your config list however you like, and use filters and sorting to find past generations quickly.

The quick menu gives you fast access to your go-to configs. Need more room? Expand to the small view. You can also open the modal from either view for a full workspace. If you want WebUI to start pre-configured, set your preferred `Startup Config` in Settings (or `None` to skip it).

## Installation

1. Open AUTOMATIC1111 WebUI.
2. Go to `Extensions > Install from URL`.
3. Paste:

```text
https://github.com/dane-9/sd-webui-state-manager-continued
```

4. Click `Install`.
5. Restart WebUI.