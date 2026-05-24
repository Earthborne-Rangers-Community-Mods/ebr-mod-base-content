# Contributing to ebr-mod-base-content

This repository is the **foundation for all Earthborne Rangers mods**. Mod
creators fork it once, then create mods as branches within their fork. It is
not a typical open-source project where you submit feature PRs.

## For Mod Creators

You do not contribute to this repo directly. Instead:

1. Fork this repository (your **mod workspace**)
2. Use `ebr new` from [ebr-mod-tools](https://github.com/Earthborne-Rangers-Community-Mods/ebr-mod-tools)
   to create mod branches
3. Edit content in Obsidian
4. Use `ebr save` to commit and push
5. Use `ebr publish` to submit your mod to the registry

See the modding guide for step-by-step instructions.

## For Shell/Infrastructure Issues

If you find a problem with the shell content on `main` (broken CSS, incorrect
folder structure, `.obsidian` config issues, or `ebr-symbols.css` rendering
bugs), you can:

1. Open an issue describing the problem
2. If you have a fix, fork and open a PR against `main`

### What Lives on `main`

The `main` branch is a thin shell containing only:

- Folder structure scaffolding
- `.obsidian/` configuration (snippets, appearance settings)
- `ebr-symbols.css` and `ebr-styles.css`
- `About this Mod.md` starter template

It contains **no campaign content**. Campaign content lives on per-campaign
branches which mod creators pull in via `ebr include`.

### What We Accept on `main`

- CSS fixes for `ebr-symbols.css` or `ebr-styles.css`
- Corrections to `.obsidian` config defaults
- Fixes to folder structure or scaffolding

### What We Do Not Accept

- Campaign content changes (those go on campaign branches, maintained by approved community members)
- New features or structural changes without prior discussion

## Reporting Issues

Open a GitHub issue for:

- Rendering bugs in `ebr-symbols.css`
- Problems with the `.obsidian` configuration
- Folder structure issues that cause problems in Obsidian

## Questions

Open a GitHub issue for questions about the base content structure or how to
build mods on top of it.
