# ebr-mod-base-content

The canonical Earthborne Rangers campaign content, formatted as an Obsidian vault. This is the **upstream repo that all mods fork from**.

## What's in here

- **Campaign content** — Markdown files for the whole official campaign guide.
- **Obsidian config** — `.obsidian/snippets/ebr-symbols.css` for rendering custom game symbols (progress, harm, sun, mountain, etc.).
- **Attachments** — images and other media referenced by the content.

## How it's used

| Role | Workflow |
|---|---|
| **Players** | You don't interact with this repo directly. The mod manager downloads mods (which are forks of this repo) for you. |
| **Mod creators** | Fork this repo to start a new mod. Edit content in Obsidian. Use `ebr-mod-tools` CLI to manage your mod. |
| **Merge-mod creators** | Fork this repo (or another mod), then use `ebr merge-from` to combine multiple mods. |

## Key conventions

- **Manifest** file paths encode structure; mod metadata lives in `ebr-mod.json`.
- **Wikilinks** (`[[Page Name]]`) for internal links when possible.
- **Custom symbols** use HTML spans styled by `ebr-symbols.css` (e.g., `<span class="progress"></span>`).
