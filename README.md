# Skills

A personal library of Claude Code skills — plus a curated, navigable map of the
best open-source skills out there. Inspired by Charlie Hills' "AI company"
approach, but built lean: install what earns its keep, build the rest myself.

> **What's a skill?** A folder with a `SKILL.md`. Its `description` tells Claude
> when to load it automatically. That's the whole mechanism.

## Layout

| Path | What's in it |
|------|-------------|
| `skills/` | My own skills (start from `skills/_template/`) |
| `docs/skill-catalog.md` | Navigation map of every skill worth knowing, by department |
| `external/` | Cloned reference repos (gitignored — study, don't ship) |
| `PLAN.md` | The staged roadmap and progress |

## My skills

### Job Search (a mini "department")

A foundation skill that learns your background once, and specialized skills that
reuse it — the same pattern Charlie's social-media library uses.

| Skill | What it does |
|-------|-------------|
| `career-profile` ⭐ | **Run first.** Learns your background from existing resumes + a short interview → writes `career-profile.md` + `achievements.md` |
| `resume-tailor` | Tailors a resume to a specific job description; honest gap-check, no fabricated metrics |
| `cover-letter` | Writes a targeted, voice-matched cover letter under 300 words |
| `linkedin-optimizer` | Rewrites headline, About, and experience bullets for your target roles |

```
career-profile ──┬──▶ resume-tailor
 (foundation)     ├──▶ cover-letter
                  └──▶ linkedin-optimizer
```

## Install a skill

Copy any skill folder into your global or project skills directory:

```bash
cp -R skills/<name> ~/.claude/skills/        # available everywhere
# or
cp -R skills/<name> /path/to/project/.claude/skills/   # one project only
```

Claude loads it automatically when your request matches its description.

## Credits

Patterns and reference skills from
[Anthropic](https://github.com/anthropics/skills),
[Superpowers (Jesse Vincent)](https://github.com/obra/superpowers), and
[Charlie Hills](https://github.com/charlie947/social-media-skills) (MIT).

## License

MIT
