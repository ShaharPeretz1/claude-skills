# Skills project — staged roadmap

Goal: use Charlie Hills' "AI company" skill set to (1) install the genuinely
useful skills, (2) build my own skills library on the same conventions, and
(3) present it all cleanly on GitHub.

Location: `~/claude-skills`

---

## Stage 1 — Install & study the real skills ✅ (done)

Cloned into `external/` (reference only — gitignored, each keeps its own history):

| Repo | What it is | Source |
|------|-----------|--------|
| `anthropic-skills` | 17 official skills incl. **skill-creator**, mcp-builder, frontend-design, web-artifacts-builder, brand-guidelines, webapp-testing | Anthropic |
| `superpowers` | Dev methodology skills: TDD, systematic-debugging, worktrees, planning, parallel agents | Jesse Vincent (obra) |
| `social-media-skills` | 17 content skills built on a `voice-builder` foundation (MIT) | Charlie Hills |
| `ai-second-brain` | Searchable second brain from chat/research history | Charlie Hills |
| `agent-harness-starter` | Scaffold for an agent harness | Charlie Hills |

See `docs/skill-catalog.md` for the full navigation map.

**Not on GitHub** (gated behind Charlie's newsletter — get later if wanted):
Marketing (45), Finance (8), Small Business (31), Legal (9), UI/UX Pro Max,
Taste, Transitions.

### To actually *use* a skill in Claude Code
Copy its folder into `~/.claude/skills/<name>/` (global) or a project's
`.claude/skills/`. Claude loads it on demand when its description matches.
Start small — install 2–3, not all of them.

---

## Stage 2 — Build my own library ⬜ (in progress)

`skills/` holds skills I own. Conventions copied from Anthropic + Charlie:
one folder per skill, a `SKILL.md` with `name` + a rich `description` (the
description is what triggers it, so make it keyword-rich).

- [x] `_template/` — starter to copy for every new skill
- [x] **Job Search department** — `career-profile` (foundation) +
      `resume-tailor`, `cover-letter`, `linkedin-optimizer`
- [ ] Level up using `skill-creator` (best meta-skill in the set)
- [ ] Next department — TBD

---

## Stage 3 — Present it on GitHub ⬜

- [x] `README.md` — org-chart storefront (the thing that earns stars)
- [ ] Create the GitHub repo + push
- [ ] Profile README ("org chart" of all my projects) — needs my handle
- [ ] Per-repo README polish across my other projects
