---
name: career-profile
description: >
  Foundation skill for the whole job-search workflow. Builds a reusable career
  profile of the user from their existing resumes, LinkedIn, and a short
  interview, saved as career-profile.md and achievements.md in the project root.
  Every other job-search skill (resume-tailor, cover-letter, linkedin-optimizer)
  reads these files, so run this FIRST. Trigger whenever the user says "set up my
  job search", "learn my background", "onboard me", "build my career profile",
  "train on my resume", or drops one or more resume/CV files into the chat.
  Produces two files: career-profile.md (facts, skills, positioning) and
  achievements.md (a bank of quantified accomplishment bullets to draw from).
---

# Career Profile

## CRITICAL: Auto-start on load

The moment this skill loads, go straight to Step 1. Do not summarize the skill
or ask permission — your first response is the intake in Step 1.

## Step 1. Gather existing material

Ask the user to point you at what they already have (accept file paths or
uploads). Look proactively in likely locations first:

- Any `*resume*.docx`, `*resume*.pdf`, `*CV*` files in the current dir, the
  Desktop, or a path the user gives
- A `linkedin-profile*.md` or exported LinkedIn PDF
- Existing cover letters (they reveal voice and priorities)

Read whatever exists. Extract: roles, dates, companies, education, hard skills,
tools, certifications, and every quantified result you can find.

## Step 2. Interview for the gaps

Only ask what the material doesn't already answer. Use AskUserQuestion for
crisp choices; free-text for stories. Cover:

1. Target roles / titles and seniority
2. Industries or mission they care about (and any to avoid)
3. Location / remote / work-authorization constraints
4. Their 2–3 strongest differentiators ("why me")
5. Any accomplishment not yet written down, especially with numbers

Keep it to one focused round; don't interrogate.

## Step 3. Write the two files

Write to the project root:

**career-profile.md**
- One-line positioning statement
- Target roles + seniority
- Constraints (location, authorization, timing)
- Skills matrix (grouped: domain, tools, methods)
- Education & certifications
- Differentiators / "why me"
- Voice notes (tone the user writes in — plain, technical, warm, etc.)

**achievements.md**
- A flat bank of accomplishment bullets, each in
  `Action → method → quantified result` form, tagged with the role and the
  skills it demonstrates. This is the reservoir resume-tailor and cover-letter
  pull from, so make it generous (aim for 15–30 bullets).

## Step 4. Confirm and hand off

Show the user the positioning line and 3 sample achievement bullets. Once they
approve, tell them the next move: "Run **resume-tailor** with a job description
to produce a targeted resume, or **cover-letter** for a letter."
