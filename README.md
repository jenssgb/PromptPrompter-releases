# PromptPrompter

<p align="center">
  <img src="icon.png" alt="PromptPrompter" width="128">
</p>

<p align="center">
  <strong>Chapter-based prompt management for live demos</strong>
</p>

<p align="center">
  <a href="https://github.com/jenssgb/PromptPrompter-releases/releases/latest">
    <img src="https://img.shields.io/github/v/release/jenssgb/PromptPrompter-releases?label=download&style=for-the-badge&t=1" alt="Download latest release">
  </a>
</p>

PromptPrompter helps you manage and deliver prompts during live technical demonstrations. Write your demo scripts as Markdown files, and PromptPrompter turns them into a navigable, copy-on-click prompter with keyboard shortcuts and a countdown timer.

## Download

**[Download the latest release](https://github.com/jenssgb/PromptPrompter-releases/releases/latest)** (Windows `.exe` installer)

No installation of Node.js or other dependencies required. Just download, install, and run.

## Features

- **Chapter-based navigation** -- each `.md` file becomes a chapter
- **One-click copy** -- click any prompt to copy it to your clipboard
- **Keyboard navigation** -- arrow keys, Enter/C to copy, E to edit
- **Split view** -- rendered Markdown context on top, active prompt below
- **Inline editing** -- add, edit, reorder, delete prompts in the UI
- **Write-back** -- edits are saved back to the source `.md` files
- **Visual editor** -- full section-based editor in a separate window
- **Markdown import** -- import existing Markdown files as new chapters
- **App badges** -- tag prompts with the app they belong to (Copilot, Excel, etc.)
- **Sidebar mode** -- compact sidebar view docked to the screen edge
- **Session timer** -- countdown timer with configurable duration
- **Always on top** -- pin the window above other apps during your demo
- **File watcher** -- auto-reloads when `.md` files change on disk
- **Dark theme** -- VS Code-inspired dark UI

## Content Format

Each `.md` file in your content folder becomes a chapter. Use fenced code blocks with `prompt` or `demo` tags:

````markdown
# My Demo

## Getting Started

### Open the App

```prompt
Create a new project called "Demo" with the default settings.
```

### Show the Dashboard

```demo
Navigate to the dashboard and point out the key metrics.
This text is displayed as instructions, not copied.
```
````

- **`prompt`** blocks are copyable text (one-click copy)
- **`demo`** blocks are presenter instructions (display only)
- The heading above each block becomes the step title

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Left` / `Right` | Navigate between prompts |
| `Up` / `Down` | Navigate between prompts |
| `Enter` / `C` | Copy current prompt |
| `E` | Enter edit mode |
| `Escape` | Exit edit / Back to menu |
| `Ctrl+K` | Search prompts |
| `Ctrl+N` | Add new prompt (edit mode) |

## Feedback

Found a bug or have a feature request? [Open an issue](https://github.com/jenssgb/PromptPrompter-releases/issues).

## License

MIT License
