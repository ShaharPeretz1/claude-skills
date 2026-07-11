---
name: template-skill
description: >
  Replace this with a rich, keyword-heavy description of WHAT the skill does and
  WHEN Claude should trigger it. This text is the only thing Claude reads to
  decide whether to load the skill, so pack it with the exact phrases a user
  would say ("build my resume", "score this post", "clean up the audio"). List
  concrete trigger words. Name any files it reads or produces.
---

# Template Skill

<!--
CONVENTIONS (learned from Anthropic's + Charlie's skills):

1. The `description` above does all the routing. Long and specific beats short.
2. If the skill should run immediately on load, add a "CRITICAL: Auto-start"
   section telling Claude to jump straight to Step 1 instead of summarizing.
3. Number your steps. Keep instructions imperative ("Ask the user X", "Write Y").
4. Store config the skill needs in predictable files (e.g. brand-kit.md,
   about-me.md) and check for them before asking the user to re-enter data.
5. Put big reference material in sibling files (reference.md, examples/) and
   point to them — don't bloat SKILL.md.
6. Use skill-creator to generate/refine this instead of writing by hand:
   copy external/anthropic-skills/skills/skill-creator into ~/.claude/skills/
-->

## Step 1. ...

## Step 2. ...
