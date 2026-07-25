# Security Policy

## Reporting a Vulnerability

This repo ships static MCP config samples and prompt text, not executable
application code, so the main risk surface is a config sample that encourages
an unsafe pattern (e.g. leaking a key, or wiring a server with excessive
permissions).

If you spot something like that, or any other security concern:

- **Preferred:** open the repo's [Security tab -> Report a vulnerability](https://github.com/M-Ashrey/claude-mcp-starter-kit/security/advisories/new) (GitHub private advisory).
- **Alternative:** email m.ashrey122@gmail.com with subject `SECURITY: claude-mcp-starter-kit`.

Please include a description of the issue and, if relevant, which file/sample it's in.

This is a solo-maintained project — there's no formal SLA, but reports are treated as priority and acknowledged as soon as I see them, typically within a few days.
