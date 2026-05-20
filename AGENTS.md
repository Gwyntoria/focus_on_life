# Repository Guidelines

## Project Structure & Module Organization

This repository is a Markdown archive for the *Focus on Life* writing project. Root files hold project metadata and lint configuration: `README.md`, `package.json`, `.markdownlint-cli2.jsonc`, `.textlintrc.json`, and `tech-terms.yml`. Main content is grouped by topic directories, such as `年度书单/`, `无谓诗/`, `飞鸟来信/`, `碎碎念/`, `翻译/`, `音乐企划/`, `闻言录/`, and `历史笔记/`. Keep images and media in the nearest relevant `assets/` folder, for example `碎碎念/assets/` or `年度书单/assets/`.

## Build, Test, and Development Commands

There is no application build step. Use these commands from the repository root:

- `npx markdownlint-cli2 --fix --no-globs path/to/file.md"`: check Markdown structure and formatting.
- `npx textlint --fix path/to/file.md"`: check prose rules, terminology, spacing, and `TODO` markers.

`package.json` currently defines no npm scripts, so call the tools with `npx` unless scripts are added later.

## Writing Style & Naming Conventions

Use Markdown for all prose. Prefer concise headings, stable Chinese punctuation, and a blank line around headings, lists, block quotes, and images. Markdown unordered lists should use `-`. Emphasis and strong emphasis should use asterisks. Avoid duplicate sibling headings. Preserve meaningful Chinese filenames for essays; use descriptive image names when adding new assets.

For mixed Chinese and Latin text, keep a space between half-width and full-width characters where the linter expects it, for example `AI 时代` rather than `AI时代`.
