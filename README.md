# Tools

Small, self-contained HTML and TypeScript tools built mostly with the help of LLMs.

Inspired by [Simon Willison's tools](https://github.com/simonw/tools) approach: each tool is a single file you can open and use immediately.

## Philosophy

- **One file per tool** — each `.html` file is self-contained (inline CSS, JS, CDN imports). No build step needed for browser tools.
- **TypeScript for CLI tools** — Node/Deno scripts live in `typescript/` when a browser isn't the right runtime.
- **Low stakes, high volume** — tools are quick to create, easy to throw away, and useful to reference later.
- **LLM-generated** — most tools are built with AI assistance. The process matters as much as the output.

## Tools

<!-- Tools will be listed here as they're added -->

## Adding a new tool

1. **Browser tool:** Create `tool-name.html` at the repo root. Keep it self-contained.
2. **CLI tool:** Create `typescript/tool-name.ts` with a shebang or run instructions.
3. Update this README with a link and one-line description.
