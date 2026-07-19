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

Want the other 5 profiles, the task templates, all 4 MCP configs, and the workflow playbooks?

---

## Get the full kit

**[→ Download the complete Claude MCP Starter Kit on Payhip](https://payhip.com/b/MlHb0)**

One-time purchase. Instant download. Free lifetime updates as new MCP servers and patterns are added.

---

## Who made this

Built and maintained by [@M-Ashrey](https://github.com/M-Ashrey). Every file in the full kit is dogfooded — the workflows here are the ones actually used to run an autonomous Claude agent day to day.

If this repo helped, a ⭐ genuinely helps others find it.

---

*Not affiliated with Anthropic. "Claude" and "MCP" (Model Context Protocol) are referenced for interoperability purposes.*
