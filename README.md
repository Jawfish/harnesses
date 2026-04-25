# LLM coding harnesses

**Plugins**: programmatic hooks like shell/code extensions triggered on lifecycle events (e.g. Claude Code hooks, opencode plugins).  
**Skills**: markdown-based prompt injection via reusable SKILL.md files invoked on demand.  
**AGENTS.md**: reads the open [AGENTS.md](https://agents.md/) instructions standard.  
**License**: client repository or distributed CLI license, not the hosted model/service license.  
**Headless**: supports non-interactive prompt execution for scripts/CI.  
**Stars**: repository star count badge served by Shields.io, cached rather than live per render.  
**LSP**: first-party or built-in Language Server Protocol support, not only a generic MCP workaround.  
**Modal**: agent modes (e.g. Plan mode, Build mode).  
**Instructions**: the tool's primary instruction/context file.

| Tool                                                      | License       | Stars                                                                                                                                                                | Lang       | OpenAI API | Multi-provider |  MCP  |  LSP  | Plugins | Skills | Modal | Headless | Subagents | Instructions |
| --------------------------------------------------------- | ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | :--------: | :------------: | :---: | :---: | :-----: | :----: | :---: | :------: | :-------: | ------------ |
| [Claude Code](https://github.com/anthropics/claude-code)  | Proprietary   | [![Stars](https://img.shields.io/github/stars/anthropics/claude-code?style=flat-square&label=%E2%98%85)](https://github.com/anthropics/claude-code/stargazers)       | TypeScript |     ✗      |       ✓        |   ✓   |   ✓   |    ✓    |   ✓    |   ✓   |    ✓     |     ✓     | CLAUDE.md    |
| [Codex](https://github.com/openai/codex)                  | Apache-2.0    | [![Stars](https://img.shields.io/github/stars/openai/codex?style=flat-square&label=%E2%98%85)](https://github.com/openai/codex/stargazers)                           | Rust       |     ✓      |       ✓        |   ✓   |   ✗   |    ✓    |   ✓    |   ✓   |    ✓     |     ✓     | AGENTS.md    |
| [Copilot CLI](https://github.com/github/copilot-cli)      | Custom ¹      | [![Stars](https://img.shields.io/github/stars/github/copilot-cli?style=flat-square&label=%E2%98%85)](https://github.com/github/copilot-cli/stargazers)               | Shell      |     ✓      |       ✓        |   ✓   |   ✓   |    ✓    |   ✓    |   ✓   |    ✓     |     ✓     | AGENTS.md    |
| [Gemini CLI](https://github.com/google-gemini/gemini-cli) | Apache-2.0    | [![Stars](https://img.shields.io/github/stars/google-gemini/gemini-cli?style=flat-square&label=%E2%98%85)](https://github.com/google-gemini/gemini-cli/stargazers)   | TypeScript |     ✓      |       ✓        |   ✓   |   ✗   |    ✓    |   ✓    |   ✓   |    ✓     |     ✓     | GEMINI.md    |
| [opencode](https://github.com/anomalyco/opencode)         | MIT           | [![Stars](https://img.shields.io/github/stars/anomalyco/opencode?style=flat-square&label=%E2%98%85)](https://github.com/anomalyco/opencode/stargazers)               | TypeScript |     ✓      |       ✓        |   ✓   |   ✓   |    ✓    |   ✓    |   ✓   |    ✓     |     ✓     | AGENTS.md    |
| [crush](https://github.com/charmbracelet/crush)           | FSL-1.1-MIT ² | [![Stars](https://img.shields.io/github/stars/charmbracelet/crush?style=flat-square&label=%E2%98%85)](https://github.com/charmbracelet/crush/stargazers)             | Go         |     ✓      |       ✓        |   ✓   |   ✓   |    ✗    |   ✓    |   ✗   |    ✓     |     ✗     | AGENTS.md ³  |
| [pi](https://github.com/badlogic/pi-mono)                 | MIT           | [![Stars](https://img.shields.io/github/stars/badlogic/pi-mono?style=flat-square&label=%E2%98%85)](https://github.com/badlogic/pi-mono/stargazers)                   | TypeScript |     ✓      |       ✓        |  ✗ ⁴  |   ✗   |    ✓    |   ✓    |   ✗   |    ✓     |     ✗     | AGENTS.md    |
| [nanocoder](https://github.com/Nano-Collective/nanocoder) | MIT           | [![Stars](https://img.shields.io/github/stars/Nano-Collective/nanocoder?style=flat-square&label=%E2%98%85)](https://github.com/Nano-Collective/nanocoder/stargazers) | TypeScript |     ✓      |       ✓        |   ✓   |   ✓   |    ✗    |   ✗    |   ✓   |    ✓     |     ✓     | AGENTS.md    |

¹ Copilot CLI's custom license permits install/run and limited unmodified redistribution, but not modification.  
² FSL-1.1-MIT is source-available with a future MIT grant.  
³ crush also reads CRUSH.md, CLAUDE.md, and GEMINI.md.  
⁴ pi intentionally omits MCP for token efficiency; it can be added via a TypeScript extension.
