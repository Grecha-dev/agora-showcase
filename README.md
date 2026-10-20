# Agora

**A local agentic AI workspace. One person + one AI pair. 6 weeks.**

Agora is a desktop + Android app where AI agents do real work: they read and write
files, run shell commands, keep memory, argue in councils, build websites in a live
preview studio, and paint images - under your control, on your machine, with your
own API keys (BYOK). No cloud account, no subscription to us: the app is local,
your data stays in a plain folder you own.

- **Demo:** screenshots below
- **Live site:** https://grecha-dev.github.io/agora-showcase/
- **Source code:** private (it's a product)

---

## What it does

**Agents with cards.** Every agent is a card: system prompt, model, connection,
toolset, avatar. Chats materialize their own model/connection at birth - no hidden
fallbacks.

**A real agentic loop.** Think, call a tool, see the result, continue.
File ops, shell with danger analysis, per-category approvals with session grants.
Custom user tools (JSON), MCP servers, skills (pinned or on a TTL shelf).

**Councils.** Group chats of 2-10 agents with per-member models, discussion rounds
and a shared table (a common workspace file). They genuinely argue.

**Memory that works.** Per-chat memory folders, automatic digests pinned right
after the system prompt, context compaction with snapshots - long chats stay sharp.

**Background jobs.** Long-running shell tasks with logs, owners, watchers and
*inheritance*: delete a chat and its jobs are adopted by a branch - or die with it,
honestly. Cron schedules included.

**Time machine.** Roll back any message - files roll back with it (git snapshots
via isomorphic-git). Full git mode per chat: init, diff, commit, push.

**Studio.** A chat that builds websites: isolated workspace, sandboxed live
preview (CSP), device frames (iPhone/Pixel/Galaxy/iPad) with real UA/touch/viewport
emulation, and a Figma-style activity feed instead of tool cards.

**Painter.** Image-gen chats with a canvas split: current image large, variant
strip below. Drag a rectangle on the canvas - the crop is described by a vision
model into tags, right into your prompt. Point editing, honestly - for pixels.

**Bridges.** Telegram / Discord / Slack - your agents live where you chat.

## The numbers

| | |
|---|---|
| Development time | **6 weeks** (Sep 7 -> Oct 20, 2026) |
| Commits | **569**, full history |
| Regression tests | **983**, run twice before every deploy |
| Dependencies | one: `isomorphic-git` |
| Team | **one human + one AI** (built in pair programming with Kimi) |

## The story

Agora is built by one person in pair with an AI. The app *is* the workflow it
implements: a human and agents sharing a workspace, files, memory and
responsibility. Every feature above shipped the same way: a real report from real
use -> implementation -> 983-test regression -> deploy to the live machine. The
commit history is the resume.

## Roadmap

Signed release APK · slash-commands for skills · Studio stage 2 (preview
selection -> edit) 

---

*Screenshots in `/screenshots`. Built with Node.js (zero-framework server),
vanilla JS frontend, Tauri 2 (desktop shell), and an AI that never sleeps.*
