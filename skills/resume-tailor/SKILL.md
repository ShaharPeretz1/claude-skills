---
name: resume-tailor
description: >
  Produce a resume tailored to a specific job description, drawing from the
  user's career-profile.md and achievements.md. Reorders and rewrites bullets to
  mirror the job's language and priorities, surfaces the most relevant
  experience first, gets past ATS keyword filters, and flags any hard
  requirement the user may not meet. Use this skill whenever the user is applying
  to a job, pastes or links a job posting, or says "tailor my resume", "resume
  for this job", "apply to this role", "customize my CV", "make my resume fit
  this", or mentions an ATS — even if they don't say the word "resume". Requires
  career-profile.md — if it is missing, run the career-profile skill first.
---

# Resume Tailor

## Step 1. Load the foundation

Read `career-profile.md` and `achievements.md` from the project root. If either
is missing, tell the user to run the **career-profile** skill first, then stop.

For the craft of ATS-safe formatting and keyword extraction, read
`references/ats-and-keywords.md` before Step 4 — it has the rules that keep the
resume machine-readable and the checklist for weaving keywords in truthfully.

## Step 2. Get the target job

Ask for the job description (paste or file/URL). Extract:

- The exact title and seniority
- Must-have requirements vs. nice-to-haves
- The 8–12 keywords/phrases that recur (skills, tools, outcomes)
- The implied priorities (what this team clearly values most)

## Step 3. Match and gap-check

Map each requirement to evidence in `achievements.md`. Produce a short internal
matrix: requirement → best-matching bullet → strength (strong/partial/none).
Call out any **must-have with no evidence** to the user honestly — don't invent
experience.

## Step 4. Assemble the tailored resume

- Lead with the summary line rewritten toward this role.
- Order sections and bullets so the strongest matches come first.
- Rewrite selected achievement bullets to echo the job's own language, keeping
  every number truthful. Never fabricate metrics or titles.
- Keep it to one page unless the user's seniority justifies two.
- Match the format of the user's existing resume if one was provided.

Output as clean Markdown (easy to paste into Docs/Word), and offer to save it as
`applications/<company>-<role>-resume.md`.

## Step 5. Report the gaps

End with a 2–3 line honesty check: which must-haves are fully covered, which are
partial, and what the user could add to strengthen the application.
