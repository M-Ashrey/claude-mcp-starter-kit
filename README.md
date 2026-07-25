# Claude MCP Starter Kit

**Turn Claude into an autonomous operator with MCP servers, battle-tested prompts, and a persistent memory system.**

Everything here was built *by* an autonomous Claude agent running the exact workflows it documents. This is not theory — it is the operating system for an AI that researches the web, ships code to GitHub, drives a browser, and remembers what it did across sessions.

---

## Why this exists

Most people use Claude like a chatbot. A few use it like an employee.

The difference is not a secret model or a jailbreak. It is **plumbing**: the right MCP servers wired up correctly, a prompt layer that makes Claude act instead of ask, and a memory file that survives context resets. Get those three right and Claude stops being a Q&A box and starts closing loops on real work.

This kit is the shortest path from "I have a Claude subscription" to "Claude just did that for me while I was asleep."

---

## What's inside the full kit

| Module | What it does |
|--------|-------------|
| `mcp-configs/` | Copy-paste JSON for 4 core MCP servers: web research, GitHub, browser automation, filesystem. Pre-wired, commented, ready to drop in. |
| `prompts/system-prompts.md` | The system-prompt layer that flips Claude from "suggests" to "does." 6 profiles for different autonomy levels. |
| `prompts/task-prompts.md` | Reusable task templates — research, build, ship, verify — with the exact phrasing that keeps Claude moving without hand-holding. |
| `workflows/memory-system.md` | The persistent memory pattern that lets Claude pick up exactly where it left off after a context reset. |
| `workflows/autonomous-loops.md` | How to structure multi-step, self-verifying task loops that don't drift or stall. |
| `QUICKSTART.md` | Zero to first autonomous task in under 15 minutes. |

---

## Free samples

Two real files from the kit are included free in this repo so you can judge the quality before buying:

1. The **Operator system prompt** (below) — flips Claude from passive to active.
2. The **web-research MCP config** (`sample/web-research.json`) — the single highest-ROI server to wire up first.

```
You are an autonomous operator, not an assistant. Your default is to ACT,
not to ask. When a task is underspecified, infer the most useful likely
intent and proceed, using your tools to discover missing details rather
than stopping to ask. Only escalate to the human for decisions that are
genuinely theirs: irreversible actions, spending money, or choices where
you cannot determine intent from context.

Before any multi-step task, check your memory file. After any meaningful
progress, write to it. Never lose state.

Close loops. A task is not done when you have a plan — it is done when the
work is verified. Run the build. Check the output. Read the result back.
```

### Quickstart: use the free sample right now

`sample/web-research.json` is a real, working MCP config — not a teaser. To use it:

1. Get a free API key from [firecrawl.dev](https://firecrawl.dev) and/or [tavily.com](https://tavily.com).
2. Clone this repo (or just copy the file):
   ```bash
   git clone https://github.com/M-Ashrey/claude-mcp-starter-kit
   cd claude-mcp-starter-kit
   ```
3. Merge the contents of `sample/web-research.json` into your Claude Desktop
   config (`claude_desktop_config.json` — on macOS:
   `~/Library/Application Support/Claude/claude_desktop_config.json`; on
   Windows: `%APPDATA%\Claude\claude_desktop_config.json`), replacing
   `fc-YOUR-KEY-HERE` / `tvly-YOUR-KEY-HERE` with your real keys.
4. Restart Claude Desktop. Ask Claude to research something on the web —
   it now has real search/scrape tools instead of relying on guesswork.

The system prompt above is also free to use as-is: paste it into Claude's
custom instructions / system prompt field to make it act instead of ask.

Want the other 5 profiles, the task templates, all 4 MCP configs, and the workflow playbooks?

---

## Get the full kit

**[→ Download the complete Claude MCP Starter Kit on Payhip](https://payhip.com/b/MlHb0)**

One-time purchase. Instant download. Free lifetime updates as new MCP servers and patterns are added.

---

## Who made this

Built and maintained by [@M-Ashrey](https://github.com/M-Ashrey). Every file in the full kit is dogfooded — the workflows here are the ones actually used to run an autonomous Claude agent day to day.

If this repo helped, a ⭐ genuinely helps others find it.

Found a broken link, a bug in the free sample, or want to report something?
Open an [issue](https://github.com/M-Ashrey/claude-mcp-starter-kit/issues). See
[SECURITY.md](SECURITY.md) to report a security concern privately.

## License

The contents of *this* repo (README, prompt text shown above, and
`sample/web-research.json`) are MIT licensed — see [LICENSE](LICENSE). The
extended paid kit sold on Payhip is a separate, commercial product.

---

*Not affiliated with Anthropic. "Claude" and "MCP" (Model Context Protocol) are referenced for interoperability purposes.*
