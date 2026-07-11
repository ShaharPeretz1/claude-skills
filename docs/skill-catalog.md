# Skill catalog — navigation map

Everything from Charlie's "42 skills" post, sorted by **who owns it** and
**how you'd actually get it**. Cloned repos live in `../external/`.

## How a skill works (30-second version)
A skill = a folder with a `SKILL.md`. The YAML `description` at the top is a
"when to use me" blurb; Claude reads all descriptions and auto-loads the skill
whose blurb matches what you're doing. Optional scripts/reference files sit
alongside. That's the whole mechanism — everything below is that pattern.

---

## Developers

| Skill | Where it really lives | Notes |
|-------|----------------------|-------|
| **Skill Creator** ⭐ | `external/anthropic-skills/skills/skill-creator` | The meta-skill. Interviews you and writes new skills. Install this first. |
| MCP Builder | `external/anthropic-skills/skills/mcp-builder` | Scaffolds MCP servers. |
| Webapp Testing | `external/anthropic-skills/skills/webapp-testing` | Drives a browser to test web apps. |
| Superpowers | `external/superpowers/skills/*` | TDD, systematic-debugging, worktrees, planning, parallel agents. Strong dev methodology. |
| Context7 | `github.com/upstash/context7` (MCP server, not a skill) | Live, version-correct library docs injected into context. |
| Claude-Mem / AI Second Brain | `external/ai-second-brain` | Persistent searchable memory from your chat/research history. |

## Designers

| Skill | Where it really lives | Notes |
|-------|----------------------|-------|
| Frontend Design | `external/anthropic-skills/skills/frontend-design` | |
| Web Artifacts | `external/anthropic-skills/skills/web-artifacts-builder` | |
| Brand Guidelines | `external/anthropic-skills/skills/brand-guidelines` | |
| UI/UX Pro Max, Taste, Transitions | Gated (Charlie's links) | Not open-source; behind his newsletter. |

## Marketing / Social / Finance / Legal / Small Business

| Collection | Status |
|-----------|--------|
| **Social Media (17)** | OPEN — `external/social-media-skills` (MIT). Built on a `voice-builder` foundation every other skill depends on. The one worth studying. |
| Marketing (45), Finance (8), Small Business (31), Legal (9) | GATED — the `lnkd.in` links are newsletter lead-magnets, not GitHub repos. Sign up to receive them. |

---

## Recommended starting set (don't install all 42)
1. **skill-creator** — so building your own is fast.
2. **superpowers** (a few: systematic-debugging, writing-plans, TDD).
3. **social-media-skills** — only if you'll publish content; study `voice-builder` regardless.
4. **ai-second-brain** — if you want memory across your research.

To install one: copy its folder into `~/.claude/skills/`.
