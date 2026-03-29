---
type: note
date: 2026-03-29
created: 2026-03-29T15:03:00Z
modified: 2026-03-29T15:03:00Z
project: p-heyron-tutorial
tags: [terminology, definitions, clarity]
---

# Terminology: Tools vs. Skills

*A clarification for tutorial readers to avoid confusion between installed tools and internal capabilities.*

---

## Tools (Installed)

**Definition:** External integrations or services that your agent can use. These live in `t-*` directories and require setup/configuration.

**Examples:**
- AgentMail (send/receive emails)
- Whisper (speech-to-text)
- here.now (web hosting)
- GitHub integration
- Cloudflare Worker

**Key point:** Tools are *optional*. You set them up based on what you need.

---

## Skills (Internal Capabilities)

**Definition:** Built-in abilities that your agent has by default. These are core functions available without installation.

**Internal Capabilities List:**

### Data & File Operations
- `read` — Read file contents
- `write` — Create or overwrite files
- `edit` — Make precise edits to files

### Computation & Execution
- `exec` — Run shell commands
- `process` — Manage background exec sessions

### Web & Information
- `web_search` — Search the web (Brave API)
- `web_fetch` — Fetch and extract readable content from URLs
- `image` — Analyze images
- `pdf` — Analyze PDF documents

### Browser & Interaction
- `browser` — Control web browser (screenshot, navigate, interact)
- `canvas` — Control node canvases (render, evaluate, snapshot)

### Device & Sensors
- `nodes` — Discover and control paired devices (camera, screen, location, notifications)

### Communication
- `message` — Send messages and channel actions (Telegram, Discord, etc.)
- `tts` — Convert text to speech

### Memory & Context
- `memory_search` — Search MEMORY.md and memory files
- `memory_get` — Safe snippet read from memory files

### Organization & Sessions
- `sessions_list` — List other sessions
- `sessions_send` — Send message to another session
- `sessions_spawn` — Spawn isolated sub-agent sessions
- `subagents` — List, kill, or steer spawned sub-agents

---

## When Talking About the Tutorial

**Tools** = things in `t-*` folders (AgentMail, Whisper, here.now, etc.)  
**Skills** = internal capabilities (web_search, web_fetch, read, write, browser control, etc.)

This distinction helps readers understand:
- Skills are free and built-in
- Tools require setup and integration
- You can start with skills, add tools as needed

---

*Last updated: 2026-03-29*
