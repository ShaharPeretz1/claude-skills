---
name: linkedin-optimizer
description: >
  Rewrite and optimize the user's LinkedIn profile for their target roles, using
  career-profile.md as the source of truth. Produces a keyword-aware headline,
  an About section in the user's voice, and tightened experience bullets that
  recruiters and LinkedIn search both reward. Trigger when the user says
  "optimize my LinkedIn", "rewrite my headline", "improve my LinkedIn profile",
  or points at a linkedin-profile file. Requires career-profile.md — run the
  career-profile skill first if it is missing.
---

# LinkedIn Optimizer

## Step 1. Load the foundation and current profile

Read `career-profile.md` and `achievements.md`. Also read any existing
`linkedin-profile*.md` or exported profile the user provides, so you improve
rather than replace what already works.

## Step 2. Confirm the target

From `career-profile.md`, restate the target roles and the 10–15 search
keywords a recruiter would type to find this person. Confirm with the user.

## Step 3. Rewrite the three high-leverage sections

1. **Headline** — not just a job title. Formula: `Role/expertise | what you do
   for whom | a proof point or specialty`. Front-load the most searched terms.
2. **About** — first two lines must hook (they show before "see more"). Written
   in the user's voice from `career-profile.md`; 3–4 short paragraphs;
   accomplishments with numbers; end with what they're looking for.
3. **Experience bullets** — tighten each role to 2–4 achievement bullets pulled
   from `achievements.md`, keyword-aware, quantified, truthful.

## Step 4. Deliver

Output each section clearly labeled and copy-paste ready. Add a short checklist
of quick wins (custom URL, banner, skills to pin, featured items). Offer to save
as `linkedin-optimized.md`.
