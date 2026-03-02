# Hone IDE

**Sharpen your code, natively.**

A native, AI-powered code editor built from scratch in TypeScript, compiled to native binaries via Perry. No Electron. No Chromium. No compromise.

> Under 50 MB · Under 100 MB RAM · Sub-second startup · 10 ms keystroke latency

---

## What makes it different

| | Hone | VSCode (Electron) |
|---|---|---|
| Cold start | < 1s | 3–5s |
| RAM idle | < 100 MB | 300–500 MB |
| Binary size | < 50 MB | ~300 MB |
| Keystroke latency | < 10 ms | 30–50 ms |

**Truly native** — Perry compiles TypeScript directly to native binaries. Every platform, no runtime overhead.

**AI-first architecture** — AI sees your syntax tree, errors, git diff, and terminal output. Deep context, not just text.

**Bring your own AI** — Claude, GPT, Gemini, Ollama, or your company's private model. Mix providers per feature. No vendor lock-in.

**Agent mode** — Describe what you want. The agent reads code, plans changes, edits files, runs tests, and iterates — with per-hunk approval before anything is committed.

**Modular and composable** — `hone-editor`, `hone-terminal`, and `hone-core` are independent packages. Use them in your own app or build your own IDE on Hone's foundation.

---

## Repositories

| Repo | Package | Status | Description |
|------|---------|--------|-------------|
| [hone-editor](https://github.com/HoneIDE/hone-editor) | `@honeide/editor` v0.2.0 | Released | Editor component — piece-table buffer, 10 languages via Lezer, LSP + DAP, ghost text, demos on macOS / iOS / Windows / Android / Web |
| [hone-terminal](https://github.com/HoneIDE/hone-terminal) | `@honeide/terminal` v0.1.0 | Released | Terminal emulator — VT100/xterm, truecolor, mouse tracking, alternate screen, OSC 133, 163 tests |
| [hone-extensions](https://github.com/HoneIDE/hone-extensions) | `@honeide/extensions` v1.0.0 | Released | Built-in language extensions — TypeScript, Python, Rust, Go, C/C++, HTML/CSS, JSON, Markdown, Git, Docker, TOML/YAML |
| [hone-themes](https://github.com/HoneIDE/hone-themes) | `@honeide/themes` v1.0.0 | Released | 11 curated themes — VSCode format compatible, WCAG contrast validated, import tools for VSCode + TextMate |
| [hone-api](https://github.com/HoneIDE/hone-api) | `@honeide/api` v0.1.0 | Released | Public extension API — zero runtime, pure TypeScript types, 452+ type-level tests |
| [hone-core](https://github.com/HoneIDE/hone-core) | `@honeide/core` v0.1.0 | In Progress | IDE services layer — workspace, file watcher, layered settings, keybindings; git / search / LSP manager and AI provider system (8 adapters) in progress |
| [hone-ide](https://github.com/HoneIDE/hone-ide) | `@honeide/ide` v0.1.0 | In Progress | Full IDE workbench — shell, file explorer, fuzzy finder, settings UI, AI setup wizard done; editor tabs, git panel, and search coming next |
| [landing](https://github.com/HoneIDE/landing) | — | Live | Marketing site at [hone.codes](https://hone.codes) |

---

## Build progress

Hone ships in 15 slices, each delivering a complete feature across all seven platforms simultaneously.

**Phase 1 — Foundation** ✓ Complete
- Slice 0: Workbench shell & theme engine
- Slice 1: Workspace & file explorer
- Slice 2: Settings, keybindings & onboarding

**Phase 2 — Core IDE** ● In Progress
- Slice 3: Editor integration *(active)*
- Slices 4–7: Git, Search, LSP & Language Intelligence, Debug

**Phase 3 — AI & Terminal** ○ Up Next
- Slices 8–13: AI provider system, inline completion, chat, terminal integration, agent mode, PR review

**Phase 4 — Extensions & Ship** ○ Planned
- Slices 14–15: Extension system, packaging (DMG, MSI, AppImage, .ipa, .apk)

---

## Contributing

- Read the [Extension API docs](https://github.com/HoneIDE/hone-api)
- Browse [built-in extensions](https://github.com/HoneIDE/hone-extensions) to see patterns
- Submit a theme via the [themes repo](https://github.com/HoneIDE/hone-themes)
