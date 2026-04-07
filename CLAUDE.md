# Tools

A collection of small, self-contained HTML and TypeScript tools.

## Structure

- Root: `.html` files — self-contained browser tools (inline CSS/JS, CDN imports, no build step)
- `typescript/`: CLI tools and Node/Deno scripts
- Each tool should be independently usable without setup

## Development Workflow

Use judgment to plan appropriately for the task:
- Simple changes: just implement directly.
- Larger changes: think through the approach before coding.
  Write a brief plan as a comment in the PR or in a scratch file,
  then implement.
- Always create a feature branch, commit with descriptive messages
  referencing the issue, and create a PR.

## Code Quality

- Write tests first when possible. Prefer test-driven development.
- Run quality checks before committing: tests, linting, type checking.
- Do not commit broken code. If tests fail, fix them before committing.
- Keep commits focused — one logical change per commit.

## Conventions

- Browser tools: single `.html` file, no external dependencies beyond CDN imports
- TypeScript tools: use Deno or tsx for execution, keep dependencies minimal
- Name files with kebab-case: `image-resizer.html`, `json-formatter.ts`
- Each tool should have a clear title and brief usage instructions embedded in it

## After Completing Work

Before wrapping up a non-trivial PR, self-assess:
- What was the hardest decision or trickiest problem?
- Did anything surprise you or require a workaround?
- Would a future session benefit from knowing this?
If yes, update CLAUDE.md with the pattern or gotcha.
