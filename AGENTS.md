# Documentation project instructions

## About this project

- This is the public documentation for Clayzo (the `clayzo` CLI, `@clayzo/animation`, `@clayzo/webgl-player`, `@clayzo/canvaskit-player` and the agent skills), built on [Mintlify](https://mintlify.com).
- Pages are MDX files with YAML frontmatter. Navigation lives in `docs.json`.
- Run `mint dev` to preview locally and `mint broken-links` to check links.
- The source of truth for behaviour is the Clayzo repository: CLI help text, package READMEs and the two agent skills. Check them before documenting a flag or option.

## Terminology

- "Document" for an animation JSON file; "bundle" for a `.clayzo` archive.
- "Player" for the browser runtimes; "WebGL player" and "CanvasKit player", never "renderer" in customer-facing text unless choosing between them.
- "Agent" for Claude Code, Cursor, Codex and similar; "skills" for the two Clayzo skills.
- "Ticks" for document time; say "ticks" not "frames" when referring to CLI options.

## Style preferences

- Active voice and second person ("you").
- One idea per sentence. Sentence case for headings.
- Code formatting for commands, file names, flags and identifiers.
- Show a command or snippet for every task; keep examples runnable.

## Content boundaries

- Document what a customer needs to install, author, preview, export and embed. Nothing else.
- Never describe engine internals: rendering pipeline, caches, schedulers, wasm, ABI, repository layout, benchmarks or internal-only CLI commands.
- Don't document unreleased features. If a flag isn't in `clayzo <command> --help`, it isn't documented.
